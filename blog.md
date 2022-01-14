---
layout: default
title: Blogs List
---


<div class="blog-card">
  {% for post in site.posts %}
    <a href="{{ post.url }}">
      <div class="blog-card-link">
        {{ post.title }}
      </div>
      <div class="blog-card-date">
        {{ post.date | date_to_string }}
      </div>
    </a>
  {% endfor %}
</div>
