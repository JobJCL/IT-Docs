---
layout: default
title: "Topdesk"
permalink: /assignments/
---

<h1>{{ page.title }}</h1>

<ul class="project-list">
  <!-- {% assign sorted_by_title = site.assignments | sort:'title' %} -->
  {% for assignment in site.assignments %}
    <li>
      <h2><a href="{{ assignment.url | relative_url }}">{{ assignment.title }}</a></h2>
      <!-- <p>{{ assignment.summary }}</p> -->
      <!-- <small>{{ assignment.date | date: "%B %d, %Y" }}</small> -->
    </li>
  {% endfor %}
</ul>
