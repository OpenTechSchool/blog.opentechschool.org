---
layout: post
title: "Presenting at Codemotion"
description: ""
category: 
tags: []

author: ben
---
{% include JB/setup %}

{% raw %}
<div id="popcorn-presentation" style="height: 400px; width: 100%">

</div>
<div id="popcorn-player" style="height:200px;">

</div>

<script src="http://popcornjs.org/code/dist/popcorn-complete.js">

</script>

<script>
var popcorn;
document.addEventListener( "DOMContentLoaded", function() {

	popcorn = Popcorn.soundcloud( "#popcorn-player", "http://soundcloud.com/sourcefabric/presentation-opentechschool-at" );

	popcorn.webpage({
	 target: 'popcorn-presentation',
	 start: 0,
	 end: 50,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#Cover"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 50,
	 end: 60,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#speakers_intro"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 60,
	 end: 85,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#tech_education"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 85,
	 end: 136,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#university"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 136,
	 end: 200,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#moocs"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 200,
	 end: 240,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#online_hands-on_coding_classes"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 240,
	 end: 314,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#P2PU"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 314,
	 end: 366,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#coding_training_schools"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 366,
	 end: 427,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#hands-on_real-life"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 427,
	 end: 457,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#opentechschool"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 457,
	 end: 541,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#open"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 541,
	 end: 589,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#empowering"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 589,
	 end: 630,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#welcoming"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 630,
	 end: 690,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#hands-on"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 690,
	 end: 748,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#not-for-profit"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 748,
	 end: 761,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#workshops"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 761,
	 end: 795,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#js-beginners"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 795,
	 end: 860,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#python-workshops"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 860,
	 end: 910,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#github-workshops"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 910,
	 end: 1002,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#android-workshops"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1002,
	 end: 1080,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#learners-meetup"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1080,
	 end: 1168,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#kids-hackathon"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1168,
	 end: 1177,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#upcoming-workshops-title"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1177,
	 end: 1370,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#upcoming-workshops"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1370,
	 end: 1395,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#further-involvements-title"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1395,
	 end: 1800,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#further-involvements"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1800,
	 end: 1810,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#not-enough"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1810,
	 end: 1870,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#one-day-to-code"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1870,
	 end: 1952,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#longer-in-depth"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 1952,
	 end: 2010,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#learning-space"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 2010,
	 end: 2080,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#bleuprint"
	}).webpage({
	 target: 'popcorn-presentation',
	 start: 2080,
	 src: "http://opentechschool.github.io/slides/presentations/the-state-of-tech-education/?full#ThankYou"
	});

}, false);
</script>

{% endraw %}
