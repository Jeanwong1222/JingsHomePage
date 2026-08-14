---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<p class="pub-intro">You can also <a href="{{ '/publications-by-topic/' | relative_url }}">browse publications by topic</a>.</p>

<div class="publications pub-byyear">

  <h2 class="pub-year">Manuscripts</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[manuscript=true] %}

  <h2 class="pub-year">2026</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2026] %}
  {% bibliography -f {{ site.scholar.bibliography }} -q @incollection[year=2026] %}

  <h2 class="pub-year">2025</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2025] %}
  {% bibliography -f {{ site.scholar.bibliography }} -q @incollection[year=2025] %}

  <h2 class="pub-year">2024</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2024] %}

  <h2 class="pub-year">2022</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2022] %}

  <h2 class="pub-year">2021</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2021] %}

  <h2 class="pub-year">2020</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[year=2020] %}

  <h2 class="pub-year">Works in Progress</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @unpublished %}

</div>
