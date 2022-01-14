---
layout: default
title: Blogs List
---


<div class="card-list">
  {% for post in site.posts %}
    <div class="blog-card">
      <a href="{{ post.url }}">
        <div class="blog-card-link">
          {{ post.title }}
        </div>
        <div class="blog-card-date">
          {{ post.date | date_to_string }}
        </div>
      </a>
    </div>
  {% endfor %}
</div>
