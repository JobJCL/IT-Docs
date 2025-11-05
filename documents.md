---
layout: default
title: "Documents"
permalink: /documents/
---

<h1>{{ page.title }}</h1>

<ul class="project-list">
  {% assign sorted_by_title = site.documents | sort:'title' %}
  {% for document in site.documents %}
    <li>
      <h2><a href="{{ document.url }}">{{ document.title }}</a></h2>
      <!-- <p>{{ assignment.summary }}</p> -->
      <!-- <small>{{ assignment.date | date: "%B %d, %Y" }}</small> -->
    </li>
  {% endfor %}
</ul>
