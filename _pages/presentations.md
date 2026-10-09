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

  <h2 id="monitoring" class="research-line line--monitoring">🚨 Real-Time Assessment Monitoring</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=monitoring] %}

  <h2 id="intervention" class="research-line line--intervention">🛡️ In-Session Intervention</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=intervention] %}

  <h2 id="item" class="research-line line--item">♻️ Continuous Item-Pool Maintenance</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=item] %}

  <h2 id="other" class="research-line line--other">Related Research in Educational Measurement and Learning</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @inproceedings[line=other] %}

</div>
