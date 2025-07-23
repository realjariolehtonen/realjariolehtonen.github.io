---
layout: page
title: Projects
permalink: /projects/
---

## 💻 Featured Projects
<ul>
  {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
  {% for project in sorted_projects limit:3 %}
    <li>
      <a href="{{ project.url }}">{{ project.title }}</a> – {{ project.description }}
    </li>
  {% endfor %}
</ul>
<p><a href="/projects">See all projects →</a></p>