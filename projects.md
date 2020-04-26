---
# front matter tells Jekyll to process Liquid
layout: default
title: "Projects"
permalink: /projects
---

<ul class="archive-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
