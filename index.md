---
layout: default
title: 9r3w's pages
---

this page is 9r3w's homepage

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
