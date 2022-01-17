---
layout: default
title: Blogs List
---


<div class="card-list">
  {% for post in paginator.posts %}
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

<!-- Pagination links -->
<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}" class="prev">
      prev
    </a>
  {% else %}
    <span class="prev">prev</span>
  {% endif %}
  <span class="page_num ">
    Page: {{ paginator.page }} of {{ paginator.total_pages }}
  </span>
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" class="next">Next</a>
  {% else %}
    <span class="next ">Next</span>
  {% endif %}
</div>
