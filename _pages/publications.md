---
layout: page
permalink: /publications/
title: Publications
nav: true
hide_title: true   # the nav tab already names the page
nav_order: 1
---
<!-- _pages/publications.md -->

<p class="pub-summary"><strong>10</strong> peer-reviewed journal articles published (<strong>5 as first author</strong>); <strong>5</strong> manuscripts under review or revision (2 as first author, 1 as co-first author); <strong>2</strong> book chapters; <strong>12</strong> conference presentations (11 as first author).</p>

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
