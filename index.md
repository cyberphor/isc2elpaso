---
layout: default
---

{% for post in site.posts %}
  <li>
    {{ post.date | date: '%B %d, %Y' }} | <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
