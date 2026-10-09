---
layout: page
permalink: /publications-by-topic/
title: Publications by Topic
nav: false
---
<!-- _pages/publications_by_topic.md -->

<p class="pub-intro">My publications are organized around three connected components of one research program. Some projects inform more than one component and are listed according to their primary decision contribution. You can also <a href="{{ '/publications/' | relative_url }}">browse publications by year</a>.</p>

<div class="publications">

  <h2 id="monitoring" class="research-line line--monitoring">🚨 Real-Time Assessment Monitoring</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[line=monitoring] %}

  <h2 id="intervention" class="research-line line--intervention">🛡️ In-Session Intervention</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @unpublished[line=intervention] %}

  <h2 id="item" class="research-line line--item">♻️ Continuous Item-Pool Maintenance</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[line=item] %}

  <h2 id="other" class="research-line line--other">Related Research in Educational Measurement and Learning</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @article[line=other] %}

  <h2 id="chapters" class="research-line line--chapter">Book Chapters</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @incollection %}

  <h2 id="wip" class="research-line line--wip">Works in Progress</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @unpublished[line!=intervention] %}

</div>
