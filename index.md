---
# front matter tells Jekyll to process Liquid
layout: default
title: "home"
permalink: /
---
<div class="right-now">
  <strong>Right now:</strong> Building pilota.io and finishing my degree (BBA Marketing & MIS) at the University of Houston.
</div>

<div>
  {% for post in site.posts limit:1 %}
    <h1>{{ post.title }}</h1>
    <p>{{ post.date }}</p>
    <div>{{ post.content }}</div>
  {% endfor %}
</div>
