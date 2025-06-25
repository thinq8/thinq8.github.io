---
layout: page
title: Projects
permalink: /projects/
---

# My Important Projects

{% assign sorted_projects = site.projects | sort: 'order' %}
{% for project in sorted_projects %}
  <div class="project">
    <h2>{{ project.title }}</h2>
    {{ project.content | markdownify }}
  </div>
{% endfor %}
