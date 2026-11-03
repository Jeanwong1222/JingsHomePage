---
layout: page
permalink: /experiences/
title: Research
nav: true
hide_title: true   # the nav tab already names the page
nav_order: 3
---
<!-- _pages/experiences.md -->

<div class="cv">
{% for entry in site.data.experiences %}
  <div class="card mt-3 p-3">
    <div>
      {% if entry.type == "time_table" %}
        {% include cv/time_table.html %}
      {% else %}
        {{ entry.contents }}
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>
