---
layout: default
---

{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
    {{ post.date | date: '%B %d, %Y' }}
  </li>
{% endfor %}
