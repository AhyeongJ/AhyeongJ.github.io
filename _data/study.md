---
layout: default
title: Study
---

# Study Posts
<ul>
  {% for post in site.posts %}
    {% if post.categories contains 'study' %}
      <li><a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}</li>
    {% endif %}
  {% endfor %}
</ul>