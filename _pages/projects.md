---
layout: page
title: research
permalink: /projects/
description: Research interests and ongoing work.
nav: true
nav_order: 2
---

## Ongoing research

{% assign sorted_projects = site.projects | sort: "importance" %}
{% for project in sorted_projects %}
  <article class="mb-4">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <p>{{ project.description }}</p>
  </article>
{% endfor %}
