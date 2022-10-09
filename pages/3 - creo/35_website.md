---
layout: page-fullwidth
#
# Content
#
subheadline: ""
title: ""
teaser: ""
comments: true
categories:
  -
tags:
  -
header: no
#
# Metainformation & Customization
#
meta_description:
permalink: "/creative-corner/website/"
---

### Why this website? <a name="siteintro"></a>

Long back, in my childhood days, my parents tried to instil in me the habit of maintaining a diary. I used to receive a new diary as a New Year gift but my enthusiasm to flip through the pages lasted only as far as my interest in the occasional glossy pages of thematic illustrations in it. A week at the most - the span of my interest to pen down the eventful moments at the end of each day. The rest of the 51 weeks were usually spent in stacking other books from school on top of the diary, till it was right at the bottom of the pile by year end.

This changed with two gradual changes in my life. The first is when Subhasis sir started to tutor me in physics (sometime in Class 8). He had an exceptionally different methodology in teaching. For me, the entire journey was like down the rabbit-hole for Alice in Wonderland. He used to tell stories which morphed physical theories from philosophical or religious principles. Though I have always been an atheist, the stories were fascinating. These were different from the stories of Hindu epics that I used to love as a lullaby from my grandma where I was a kid. These were bold conjectures - mostly unprovable. Let me give you an example. Some even lunatic. Why is gravity always attracting? Well, no one knows! We can call it a property of the Higgs boson, or pi meson exchange, or ... well, we can keep guessing. But, we can also say, all mass for the Newtonian equation are complex numbers. Lo and behold! That would always result in the negative sign for attraction. Yes, it might sound completely nuts, but, this was the first time I felt, I needed to note this down somewhere safe, that would outlive my class notes past the academic year. This was the first time I actually started writing a diary. A diary of random thoughts. Mostly based on the stories that sir used to tell me.

The second change came much more recently with social media feeds. Facebook (and to some extent LinkedIn, Pinterest, etc.) that built a network of people with a diversity of ideas. And some of these ideas were as crazy as sir's. Of course, I didn’t need a diary for these. I can always share them in my feed and search for them later. Yet again, some of these ideas really stood out. They were too important for me – my personal aspiration to understand the secrets to the treasure trove of the Universe. I needed a more organised personal space – a mind palace like Sherlock's if you will. So though this venture has long lingered at the bottom of my to-do list, it is time to piece together these thoughts into a coherent mess!

I write with the hope that it would stimulate the occasional visitors to see the World with a different eye.

When was the last time you stopped in your busy lives, thinking of how the World we live in looks like, sounds like, and most of all, feels like. Shackled in the clutches of our busy routine, we forget to smile at the babies wailing to get our attention. The babies inside us all. We ignore them until we are old enough to understand that we are now too old. Take a few minutes off from the tomorrow's schedule and enjoy the present.

Do we really see the World the way it is? Or is the World the way we see it?

### This Website

Some links that I am yet to explore, or found useful in the making of this website:
* [HTML5 games on GitHub Pages](https://end3r.com/blog/2014/02/host-your-html5-games-on-github-pages/)
* [Mathjax parsed with Jekyll](https://stackoverflow.com/questions/34227995/mathjax-being-parsed-with-jekyll/34231579#34231579)
* Plotly
* [The Executable Books Project](https://executablebooks.org/en/latest/)

### Sandbox

The space below is where I try these new features.

##### Embed image from google drive

<iframe src="https://drive.google.com/file/d/1OmGLCECAYAhNzHuDDrNzGMUvwPbWv3a6/preview" width="640" height="480" allow="autoplay"></iframe>

##### Wolfram API

<script type="text/javascript" id="WolframAlphaScript5d3dce72cfeaf05c96e2939b9c7ead33" src="//www.wolframalpha.com/widget/widget.jsp?id=5d3dce72cfeaf05c96e2939b9c7ead33"></script>

##### Google Search

{% include _google_search.html %}

##### Interactive

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