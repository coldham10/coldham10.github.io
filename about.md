---
layout: post
title: About Me
description: Get to know me personally
image: assets/images/memountain.jpg
nav-menu: true
---

Hi, I'm Christopher Oldham, a traveller, developer, science lover, explorer and global citizen. I am from New Zealand and the US, and have lived in Guatemala, Sri Lanka, Mexico, Russia and Colombia as well.

Since 2019 I have finished my undergrad degrees in physics and computer science and engineering; wrote my [thesis]({% post_url 2019-10-1-scarborsnv %}); travelled in Asia and South America; been locked down multiple times; wrote an Android app and moved to London.

I am now looking for a job in software engineering or data science at a company solving interesting and important problems. My favourite programming languages are Python and C, but I'm handy in Java and JavaScript (+React) as well, and I have experience with ML frameworks including TensorFlow and Torch. I speak English natively and Spanish proficiently; in my spare time I like to read non-fiction, play guitar and jog with friends.

<hr class="major" />

## Twenty, Twenty-one...

The 2020 pandemic cut my travels in South America short and I went home to spend lockdown with my family. After some smaller projects and online study, I decided to build a [website]({% post_url 2020-6-1-cvingles %}) and an [app]({% post_url 2021-1-1-continuum %}). At the start of this somewhat uncertain year I am now looking for the perfect job in software engineering or data science - one in which I am playing my small part in improving the fate of our world. I am keen to work for any company that is trying to solve world or regional problems, but a few areas I currently find really interesting are:

- Responsible AI development
- Mitigating the worst effects of climate change
- New techniques in machine learning (incl. GANs and GCNs)
- Bioinformatics and computational physics
- Effective altruism and global coordination problems

<hr class="major"/>

### My Travel Map

<script src="https://www.amcharts.com/lib/3/ammap.js" type="text/javascript"></script>
<script src="https://www.amcharts.com/lib/3/maps/js/worldHigh.js" type="text/javascript"></script>
<script src="https://www.amcharts.com/lib/3/themes/dark.js" type="text/javascript"></script>
<div id="mapdiv" style="width: 1000px; height: 450px;"></div>
<script type="text/javascript">
var map = AmCharts.makeChart("mapdiv",{
type: "map",
theme: "dark",
projection: "lambert",
panEventsEnabled : true,
backgroundColor : "#535364",
backgroundAlpha : 0.25,
zoomControl: {
zoomControlEnabled : true
},
dataProvider : {
map : "worldHigh",
getAreasFromMap : true,
areas :
[
	{
		"id": "BE",
		"showAsSelected": true
	},
	{
		"id": "BG",
		"showAsSelected": true
	},
	{
		"id": "CZ",
		"showAsSelected": true
	},
	{
		"id": "FR",
		"showAsSelected": true
	},
	{
		"id": "DE",
		"showAsSelected": true
	},
	{
		"id": "GR",
		"showAsSelected": true
	},
	{
		"id": "IT",
		"showAsSelected": true
	},
	{
		"id": "NL",
		"showAsSelected": true
	},
	{
		"id": "PT",
		"showAsSelected": true
	},
	{
		"id": "RU",
		"showAsSelected": true
	},
	{
		"id": "ES",
		"showAsSelected": true
	},
	{
		"id": "CH",
		"showAsSelected": true
	},
	{
		"id": "TR",
		"showAsSelected": true
	},
	{
		"id": "GB",
		"showAsSelected": true
	},
	{
		"id": "VA",
		"showAsSelected": true
	},
	{
		"id": "CA",
		"showAsSelected": true
	},
	{
		"id": "SV",
		"showAsSelected": true
	},
	{
		"id": "ID",
		"showAsSelected": true
	},
	{
			"id": "SG",
			"showAsSelected": true
	},
	{
		"id": "DO",
		"showAsSelected": true
	},
	{
		"id": "GT",
		"showAsSelected": true
	},
	{
		"id": "MX",
		"showAsSelected": true
	},
	{
		"id": "US",
		"showAsSelected": true
	},
	{
		"id": "CO",
		"showAsSelected": true
	},
	{
		"id": "EG",
		"showAsSelected": true
	},
	{
		"id": "MA",
		"showAsSelected": true
	},
	{
		"id": "CN",
		"showAsSelected": true
	},
	{
		"id": "HK",
		"showAsSelected": true
	},
	{
		"id": "IN",
		"showAsSelected": true
	},
	{
		"id": "MY",
		"showAsSelected": true
	},
	{
		"id": "NP",
		"showAsSelected": true
	},
	{
		"id": "KR",
		"showAsSelected": true
	},
	{
		"id": "LK",
		"showAsSelected": true
	},
	{
		"id": "TH",
		"showAsSelected": true
	},
	{
		"id": "AE",
		"showAsSelected": true
	},
	{
		"id": "VN",
		"showAsSelected": true
	},
	{
		"id": "AU",
		"showAsSelected": true
	},
	{
		"id": "NZ",
		"showAsSelected": true
	}
]
},
areasSettings : {
autoZoom : true,
color : "#B4B4B7",
colorSolid : "#84ADE9",
selectedColor : "#84ADE9",
outlineColor : "#666666",
rollOverColor : "#9EC2F7",
rollOverOutlineColor : "#000000"
}
});
</script>
