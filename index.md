---
layout: bare
title: Home
---

# Welcome to My Homepage

This site showcases my blog articles and software projects. Stay tuned for updates!

## 📝 Latest Blog Posts

<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> – {{ post.date | date: "%B %d, %Y" }}<br/>
      <small>{{ post.description }}</small>
    </li>
  {% endfor %}
</ul>
<p><a href="/blog">Read all posts →</a></p>

## 💻 Featured Projects
<ul>
  {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
  {% for project in sorted_projects limit:3 %}
    <li>
      <a href="{{ project.url }}">{{ project.title }}</a> – {{ project.description }}
    </li>
  {% endfor %}
</ul>