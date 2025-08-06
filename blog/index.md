---
layout: clean
title: Blog
permalink: /blog/
---

# Blog

Here are all the published blog posts:

<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}</li>
  {% endfor %}
</ul>