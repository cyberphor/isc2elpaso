---
layout: default
title: 'Blog'
permalink: 'blog'
---

## Blog
<ul class="posts-list">
  {% for post in site.posts %}
    {% if post.category == 'post' %}
      <li>
        {{ post.date | date: '%B %d, %Y' }} | <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endif %}  
  {% endfor %}
</ul>
