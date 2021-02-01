---
layout: post
title: Continuum
description: Habit Tracking React Native App
image:
permalink: /projects/Continuum
---

I heard a talk by author James Clear on the critical importance of habits in almost every aspect of life, and I became quite interested in the [interplay between goals and habits](https://psycnet.apa.org/doi/10.1037/0033-295X.114.4.843){:target="\_blank"}. However despite my best attempts to form new habits and break old ones, I found myself struggling to be sure of how well I was doing. Had I really been keeping up with new habits? How long had I abstained from those bad habits? Did I do push-ups this morning, or was that yesterday? Pen and paper helped somewhat but came with its own issues: not only keeping track of the tallies, but ironically logging habits is not the easiest habit to maintain.

What I needed was an app with a simple, intuitive UI that would remind me to log my habits and let me see how I was doing at a glance. Instead of finding the perfect app, I had just taught myself JavaScript and React and so I decided to write one myself using React Native.

Intuitively I find that making good habits and breaking bad habits follow different patterns. If I've gone running every day for a week, after a day off I still have a lot of momentum to keep exercising. Reverting to an old bad habit feels a lot more like "falling off the wagon," no matter how trivial the habit. I translated this intuitive notion of "momentum" into mathematical formulae, which I coded up in turn, and I was off!

<div class="box">
	<div class="row 50% uniform">
		<div class="6u 12u$(medium)"><h4>Positive habit momentum</h4><span class="image fit"><img src="{% link assets/images/positive.jpg %}" alt="" /></span></div>
		<div class="6u 12u$(medium)"><h4>Negative habit momentum</h4><span class="image fit"><img src="{% link assets/images/negative.jpg %}" alt="" /></span></div>
	</div>
  <br/>
  <p>Comparison of positive habit momentum function vs negative habit momentum function for a user who maintains (or abstains from) the habit for 10 days, forgets for a few days and then starts again.</p>
</div>

Handily the rate at which momentum builds up (and falls away in the case of positive habits) can be parameterised as a time in days - giving the user an intuitive way to control how each habit works for them. The rest of the project was learning the various quirks and good UX decisions of React Native and Android, and finding all the additional packages to do what I needed. For this project I also decided to use [Redux](https://redux.js.org/){:target="\_blank"} to store all the habit and settings data in a predictable, persistable way.

On Android you can download the beta [here](https://play.google.com/store/apps/details?id=com.tripconey.continuum){:target="\_blank"}, and the source can be found [on my GitHub](https://github.com/coldham10/Continuum){:target="\_blank"}.
