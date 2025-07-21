---
layout: default
title: Home
---

# Welcome to My Homepage

This site showcases my blog articles and software projects. Stay tuned for updates!

## 📝 Latest Blog Posts

<ul>
  {% for post in site.posts limit:3 %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}</li>
  {% endfor %}
</ul>
<p><a href="/blog">Read all posts →</a></p>

## 💻 Featured Projects

<ul>
  <li><a href="https://github.com/realjariolehtonen/project1">Project 1</a> – Short description of Project 1.</li>
  <li><a href="https://github.com/realjariolehtonen/project2">Project 2</a> – Short description of Project 2.</li>
</ul>
<p><a href="/projects">See all projects →</a></p>