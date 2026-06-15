---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<p class="pub-intro">Journal articles, organized by my three research directions and listed in reverse-chronological order within each.</p>

<div class="publications">

  <h2 id="examinee" class="research-line line--examinee">🚨 Real-Time Examinee Monitoring</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[line=examinee] %}

  <h2 id="item" class="research-line line--item">🔍 Real-Time Item Health</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[line=item] %}

  <h2 id="pool" class="research-line line--pool">♻️ Real-Time Pool Replenishment</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[line=pool] %}

  <h2 id="other" class="research-line line--other">Other Research</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[line=other] %}

  <h2 id="chapters" class="research-line line--chapter">Book Chapters</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @incollection %}

  <h2 id="wip" class="research-line line--wip">Works in Progress</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @unpublished %}

</div>
