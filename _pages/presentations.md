---
layout: page
permalink: /presentations/
title: Presentations
nav: true
nav_order: 2
---
<!-- _pages/presentations.md -->

<p class="pub-intro">Conference presentations, organized by my three research directions and listed in reverse-chronological order within each.</p>

<div class="publications presentations-list">

  <h2 id="examinee" class="research-line line--examinee">🚨 Real-Time Examinee Monitoring</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=examinee] %}

  <h2 id="item" class="research-line line--item">🔍 Real-Time Item Supervision</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=item] %}

  <h2 id="pool" class="research-line line--pool">♻️ Real-Time Pool Replenishment</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=pool] %}

  <h2 id="other" class="research-line line--other">Other Research</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=other] %}

</div>
