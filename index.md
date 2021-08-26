---
# front matter tells Jekyll to process Liquid
layout: default
title: "home"
permalink: /
---
<div class="row">
  <div class="col-9">
    {% for post in site.posts %}
      <li class="post-title">
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
      <div class="row">
        <div class="col-2">
          <p class="post-date">
            <ion-icon name="calendar-clear-outline" class="calendar-clear-outline"></ion-icon>
            <span class="text">{{ post.date | date: "%B %Y" }}</span>
          </p>
        </div>
        <div class="col-2">
          <p class="post-time"><ion-icon name="time-outline" class="time-outline"></ion-icon>{{ post.time }}</p>
        </div>  
        <div class="col-8">
        </div>
      </div>
    {% endfor %}
    </div>
    <div class="col-3 home-bio">
      <img src="/assets/img/profile-photo.svg" class="profile-photo">
      <h4 class="bio-name">Rob Dudley</h4>
      <p class="title"><b>Student & UX Designer</b></p>
      <p class="about">Currently finishing my degree<br> (BBA in Marketing and Management Information Systems, Fall '21)<br></p>
        <a href="https://www.linkedin.com/in/robwdudley" target="_blank">
          <button type="button" class="btn-linkedin">
            <ion-icon name="logo-linkedin" class="logo-linkedin"></ion-icon>
              Connect
          </button>
        </a>
    </div>
</div>
