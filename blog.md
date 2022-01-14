---
layout: default
title: Blogs List
---


<div class="blog-card">
  {% for post in site.posts %}
    <div class="blog-card-link">
      <a href="{{ post.url }}">{{ post.title }}</a>
    </div>
    <div class="blog-card-date">
      {{ post.date | date_to_string }}
    </div>
  {% endfor %}
</div>
