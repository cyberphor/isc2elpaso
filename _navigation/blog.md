---
layout: default
title: 'Blog'
permalink: 'blog'
---

## Blog
<ul class="posts-list">
  {% for post in site.posts %}
    {% if post.category == 'post' %}
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> {{ post.date | date: '%B %d, %Y' }}
    {% endif %}  
  {% endfor %}
</ul>
