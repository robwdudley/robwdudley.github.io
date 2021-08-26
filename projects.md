---
# front matter tells Jekyll to process Liquid
layout: single-page
title: "Projects"
permalink: /projects
---

<ul class="projects-list">
{% for project in site.data.projects %}
  <li>
  <a href="{{ project.url }}">  <div class="row">
      <span class="project-name">{{ project.name }}</span>
    </div> </a>
    {% if project.image %}
<a href="{{ project.url }}">      <div class="row">
        <img src="{{ project.image }}" class="project-image">
      </div>  </a>
    {% endif %}
    <div class="row category">
       {{ project.category }}
    </div>
    <div class="row summary">
      {{ project.summary }}
    </div>
  </li>
  <hr style="margin-top: 2em"/>
{% endfor %}
</ul>
