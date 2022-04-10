---
layout: page-fullwidth
title: "Creō"
meta_title: ""
subheadline: ""
teaser: ""
comments: true
header:
   image_fullwidth: "page_head/creativecorner.jpg"
permalink: "/creative-corner/"

widget1:
  title: "The Night Is Long"
  url: 'https://prince-ph0en1x.github.io/creative-corner/the-night-is-long/'
  image: page_head/poems.jpg
  text: 'collection of poems'
widget2:
  title: "Sargam"
  url: 'https://prince-ph0en1x.github.io/creative-corner/music/'
  image: page_head/music.jpg
  text: 'musical journey'
widget3:
  title: "Artfulness"
  url: 'https://prince-ph0en1x.github.io/creative-corner/art-n-craft/'
  image: page_head/art.jpg
  text: 'art and craft'
widget4:
  title: "Clichik"
  url: 'https://prince-ph0en1x.github.io/creative-corner/photography/'
  image: page_head/photography.jpg
  text: 'photography'
widget5:
  title: "Recipies"
  url: 'https://prince-ph0en1x.github.io/creative-corner/recipes/'
  image: page_head/recipies.jpg
  text: '(under construction)'
---

Here I intend to curate my creative ventures.

<div class="row t60">
	{% include _frontpage-widget.html widget=page.widget1 %}
	{% include _frontpage-widget.html widget=page.widget2 %}
	{% include _frontpage-widget.html widget=page.widget3 %}
</div>

<div class="row t60">
	{% include _frontpage-widget.html widget=page.widget4 %}
	{% include _frontpage-widget.html widget=page.widget5 %}
</div>

## This Website

Some links that I am yet to explore, or found useful in the making of this website:
* [HTML5 games on GitHub Pages](https://end3r.com/blog/2014/02/host-your-html5-games-on-github-pages/)
* [Mathjax parsed with Jekyll](https://stackoverflow.com/questions/34227995/mathjax-being-parsed-with-jekyll/34231579#34231579)
* Plotly

## Sandbox

The space below is where I try these new features.

### Embed image from google drive

<iframe src="https://drive.google.com/file/d/1OmGLCECAYAhNzHuDDrNzGMUvwPbWv3a6/preview" width="640" height="480" allow="autoplay"></iframe>

### Wolfram API

<script type="text/javascript" id="WolframAlphaScript5d3dce72cfeaf05c96e2939b9c7ead33" src="//www.wolframalpha.com/widget/widget.jsp?id=5d3dce72cfeaf05c96e2939b9c7ead33"></script>

### Google Search

{% include _google_search.html %}

### Interactive

<div id="errors" style="
  background: #c00;
  color: #fff;
  display: none;
  margin: -20px -20px 20px;
  padding: 20px;
  white-space: pre-wrap;
"></div>
<div id="root"></div>
<script>
window.addEventListener('mousedown', function(e) {
  document.body.classList.add('mouse-navigation');
  document.body.classList.remove('kbd-navigation');
});
window.addEventListener('keydown', function(e) {
  if (e.keyCode === 9) {
    document.body.classList.add('kbd-navigation');
    document.body.classList.remove('mouse-navigation');
  }
});
window.addEventListener('click', function(e) {
  if (e.target.tagName === 'A' && e.target.getAttribute('href') === '#') {
    e.preventDefault();
  }
});
window.onerror = function(message, source, line, col, error) {
  var text = error ? error.stack || error : message + ' (at ' + source + ':' + line + ':' + col + ')';
  errors.textContent += text + '\n';
  errors.style.display = '';
};
console.error = (function(old) {
  return function error() {
    errors.textContent += Array.prototype.slice.call(arguments).join(' ') + '\n';
    errors.style.display = '';
    old.apply(this, arguments);
  }
})(console.error);
</script>


