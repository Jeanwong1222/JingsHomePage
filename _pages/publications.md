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

<script>
document.addEventListener('DOMContentLoaded', function () {
  document.querySelectorAll('.pub-byyear .pub-box ol.bibliography').forEach(function (ol) {
    // Count down so the newest (top) entry carries the largest number,
    // making the total publication count visible at a glance.
    ol.setAttribute('reversed', 'reversed');
    // Widen the gap wherever the publication year changes.
    var prevYear = null;
    ol.querySelectorAll(':scope > li').forEach(function (li) {
      var per = li.querySelector('.periodical');
      var text = per ? per.textContent : li.textContent;
      var m = text.match(/\b(20|19)\d{2}\b/);
      var year = m ? m[0] : null;
      if (prevYear !== null && year !== null && year !== prevYear) {
        li.classList.add('year-break');
      }
      if (year !== null) prevYear = year;
    });
  });
});
</script>
