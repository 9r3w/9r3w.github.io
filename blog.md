---
layout: default
title: Blogs List
---


<div class="card-list">
  {% for post in site.posts %}
    <div class="blog-card">
      <div class="blog-card-link">
        <a href="{{ post.url }}">
          {{ post.title }}
        </a>
      </div>
      <div class="blog-card-date">
        {{ post.date | date_to_string }}
      </div>
      <div class="blog-card-expt">
        {{ post.excerpt }}
      </div>
      <a href="{{ post.url }}">
        read more
      </a>
    </div>
  {% endfor %}
</div>
