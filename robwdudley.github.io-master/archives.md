---
# front matter tells Jekyll to process Liquid
layout: single-page
title: "Archives"
permalink: /archives
---

<ul class="archive-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
