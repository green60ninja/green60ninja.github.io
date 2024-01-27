---
title: Home
layout: default
---
# Welcome to my website!

Here, you can find information about me, projects I have done, and my résumé.

<ul>
  {% for post in site.posts %}
  <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
  <span>{{ post.date | date_to_string }}</span>
  {% endfor %}
</ul>
