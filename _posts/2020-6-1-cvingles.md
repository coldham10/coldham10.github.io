---
layout: post
title: CVInglés
description: CV Translation, Copy Editing and Typesetting website
image:
permalink: /projects/CVIngles
---

I have always quite liked reviewing my friends' and colleagues' CVs. Since I learned to use the LaTeX typesetting language to write reports for my physics degree, I can also usually make CVs look cleaner and more professional than those written in a word processor. When I was living in Colombia at the beginning of 2020, my friend and I had an idea to turn this hobby into a business &mdash; reviewing, copy editing, translating and typesetting CVs for Latin Americans seeking work in English-speaking countries.

I wanted to start learning web development, so I took the opportunity to learn HTML, CSS and vanilla JavaScript and then quickly decided to learn React and JSX as well. I had learned about Amazon Web Services working on a media processing project with a digital signage company while at university, so I decided to write a back end and data processing pipeline for the website using only AWS microservices.

The website would be hosted using the AWS CloudFront CDN, and form submission would send a JSON object to an AWS API Gateway endpoint to be stored in an S3 bucket. When a successful payment webhook from Stripe triggered another API endpoint, the stored JSON file would be translated into a LaTeX file of the CV by a Python script in an AWS Lambda function.

Once I got the basic pipeline working I also added the ability for the user to upload a photo of themselves. I resized large images on the client side first, before sending the image to yet another API Gateway endpoint to be stored in another S3 bucket. If a photo had been uploaded, when processing the form data another Python Lambda would crop the image to square and send the new image to the "processed" S3 bucket along with the LaTeX .tex file.

The final step for the back end was to include machine translation using Amazon Translate. If translation had been requested and paid for, another Python Lambda would translate the relevant values of the original JSON object, before running the same LaTeX-generating Lambda on the machine-translated JSON file.

At the end of the pipeline I used an AWS SQS queue to make sure every Lambda that needed to run had run. At that point a final Lambda script zipped together (at most) the original .tex file, the translated .tex file and the cropped and resized image before sending that zip file to the company email address using AWS SES. The raw and processed files were deleted from the S3 buckets automatically after 30 days.

The client id; payment id and status; service requested; IP address; processing status and file names for the image and JSON form data were tracked and stored in a NoSQL AWS DynamoDB database. I also wrote a simple email proxy server using SES and Lambdas so customers could send question emails to an address with the same domain as the website, and I could respond from the company @gmail account without the customer ever noticing.

After having to leave Colombia at the beginning of COVID-19, I no longer had such easy access to native Spanish speakers willing to help start the company. Alone, my Spanish isn't good enough to maintain the professionalism and trust needed by customers to send money to a website to help them with their CV. Because of this the website never went live. All the React code for the front end is on my GitHub [here](https://github.com/coldham10/cvingles_react_app), and the back end code for the Lambdas (and a diagram of how they are interlinked) can be found [here](https://github.com/coldham10/CVIngles_Lambdas).
