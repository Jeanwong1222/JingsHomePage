---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<p class="pub-intro">Journal articles and book chapters, listed in reverse-chronological order. You can also <a href="{{ '/publications-by-topic/' | relative_url }}">browse publications by topic</a>.</p>

<div class="publications">

  <h2 class="year">Works in Progress</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @unpublished %}

  <h2 class="year">Under Review / In Revision</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2026] %}

  <h2 class="year">2025</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2025] %}

  <h2 class="year">2024</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2024] %}

  <h2 class="year">2022</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2022] %}

  <h2 class="year">2021</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2021] %}

  <h2 class="year">2020</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2020] %}

  <h2 class="year">Book Chapters</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @incollection %}

</div>
