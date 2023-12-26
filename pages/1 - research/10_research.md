---
layout: page-fullwidth
title: ""
meta_title: ""
subheadline: ""
teaser: ""
comments: true
header: no
image: no
#    title: "research/scientists.jpg"
#    caption: "3 of my favourite scientists: John von Neumann, John Archibald Wheeler, Ray Solomonoff"
#    caption_url:
permalink: "/research/"

widget1:
  title: "Research Interests"
  url: 'https://aritrasarkar.com/research/interests/'
  image: research/r01.jpg
  text: ''
widget2:
  title: "Projects & Publications"
  url: 'https://aritrasarkar.com/research/projects/'
  image: research/r02.jpg
  text: ''
widget3:
  title: "Teaching & Outreach"
  url: 'https://aritrasarkar.com/research/presentations/'
  image: research/r03.jpg
  text: ''
widget4:
  title: "Curriculum Vitae"
  url: 'https://aritrasarkar.com/research/cv/'
  image: research/r04.jpg
  text: ''
---

<body style="background-color:#F0F0FF;"></body>

<div class="medium-12 medium-pull-0 columns" markdown="1" style='text-align: left;'>

<div class="row t60">
	{% include _frontpage-widget.html widget=page.widget1 %}
	{% include _frontpage-widget.html widget=page.widget2 %}
</div>

<div class="row t60">
	{% include _frontpage-widget.html widget=page.widget3 %}
	{% include _frontpage-widget.html widget=page.widget4 %}
</div>

<!--
* [Research Interests](https://aritrasarkar.com/research/interests/)
* [Projects](https://aritrasarkar.com/research/projects/)
* [Curriculum Vitae](https://aritrasarkar.com/research/cv/)
* [Teaching and Outreach](https://aritrasarkar.com/research/presentations/)
-->

<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-136827293-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-136827293-1');
</script>
