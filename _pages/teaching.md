---
layout: page
permalink: /teaching/
title: Teaching
nav: true
hide_title: true   # the card already carries the section heading
nav_order: 4
---
<!-- _pages/teaching.md -->

<div class="cv">
{% for entry in site.data.teaching %}
  <div class="card mt-3 p-3">
    <h3 class="card-title font-weight-medium">{{ entry.title }}</h3>
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
