---
title: Projects
layout: landing
description: "A sample of my projects that I'm most excited about"
image: assets/images/Project_banner.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h2>Always Tinkering</h2>
		</header>
		<p>From analyzing COVID-19 data and predicting turning points, to writing CLI-based screensavers for a Raspberry Pi, to attempting automated crossword-puzzle building &mdash; I'm always trying things, learning, and building something. My more major projects make it on to my GitHub, of which the following are my favourites.</p>
	</div>
</section>

<!-- Two -->
<section id="two" class="spotlights">
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/continuum_collage.jpg %}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Continuum Android App</h3>
				</header>
				<p>After becoming interested in the interplay between goals and habits, I found myself struggling to remember how well I had been keeping up with new habits and how long I had abstained from bad habits. I had just taught myself JavaScript and React, so I decided to write a React Native app to help me keep track. Continuum is now available as a beta on the Android Play Store.</p>
				<ul class="actions">
					<li><a href="{% post_url 2021-1-1-continuum %}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/SCarborSNV.jpg %}" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>SCarborSNV Genetic Variant Caller</h3>
				</header>
				<p>A novel bioinformatics tool that became my undergraduate honors thesis. A probabilistic phylogeny-aware algorithm, implemented in C that finds single-letter mutations in DNA from sequence data. Up for a challenge? <a href="/assets/SCarborSNV.pdf" download>Read the thesis</a>.</p>
				<ul class="actions">
					<li><a href="{% post_url 2019-10-1-scarborsnv %}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="{% link assets/images/CVIngles.jpg %}" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>CVInglés Website</h3>
				</header>
				<p>A CV design website aimed at Latin Americans seeking work in English speaking countries. Services include copy editing English language submissions, professional translation of Spanish language submissions, in-depth consultation, and typesetting in LaTeX. The front end is written in React and the back end uses AWS APIs and microservices (especially Lambda) to automate payment confirmation, image processing, initial machine translation and the generation of .tex files that can be compiled into PDF documents.</p>
				<ul class="actions">
					<li><a href="{% post_url 2020-6-1-cvingles %}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
</section>

</div>
