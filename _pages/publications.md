---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<p class="pub-intro">Listed in reverse-chronological order. You can also <a href="{{ '/publications-by-topic/' | relative_url }}">browse publications by topic</a>.</p>

<div class="publications pub-byyear">

  <h2 class="pub-section">Journal Articles</h2>
  <div class="pub-box">
  {% bibliography -f {{ site.scholar.bibliography }} -q @article %}
  </div>

  <h2 class="pub-section">Book Chapters</h2>
  <div class="pub-box">
  {% bibliography -f {{ site.scholar.bibliography }} -q @incollection %}
  </div>

  <h2 class="pub-section">Works in Progress</h2>
  <div class="pub-box">
  {% bibliography -f {{ site.scholar.bibliography }} -q @unpublished %}
  </div>

</div>
