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
// Applies spacing + reversed numbering as INLINE styles so the layout is
// correct even when an old main.css is still cached by the browser/CDN.
document.addEventListener('DOMContentLoaded', function () {
  document.querySelectorAll('.pub-byyear .pub-box ol.bibliography').forEach(function (ol) {
    // Count down so the newest (top) entry carries the largest number,
    // surfacing the total publication count at a glance.
    ol.setAttribute('reversed', 'reversed');

    var items = ol.querySelectorAll(':scope > li');
    var prevYear = null;
    items.forEach(function (li) {
      // Tight gap between entries of the same year.
      li.style.marginBottom = '0.3rem';

      var per = li.querySelector('.periodical');
      var text = per ? per.textContent : li.textContent;
      var m = text.match(/\b(20|19)\d{2}\b/);
      var year = m ? m[0] : null;

      // Wider gap whenever the publication year changes.
      if (prevYear !== null && year !== null && year !== prevYear) {
        li.style.marginTop = '1.7rem';
      }
      if (year !== null) prevYear = year;
    });
  });
});
</script>
