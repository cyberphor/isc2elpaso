---
layout: default
title: 'Events'
permalink: 'events'
---

## Events
<ul class="notes-list">
  {% assign sorted_posts = site.posts | sort: 'title' %}
  {% for post in sorted_posts %}
    {% if post.category == 'event' %}
      <li>
        <a href="{{ post.url | relative_url }}">
          {{ post.title }}
        </a>
        {{ post.date }}
      </li>
    {% endif %}
  {% endfor %}
</ul>
