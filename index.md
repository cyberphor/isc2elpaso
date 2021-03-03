---
layout: default
---

![El-Paso-Logo.jpg]({{ site.url }}{{ site.baseurl }}/_assets/El-Paso-Logo.jpg)

<ul class="notes-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
