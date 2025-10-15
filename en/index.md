---
layout: default
title: "English"
permalink: /en/
---

# English posts

<ul class="post-list">
{% assign posts_en = site.posts | where: "lang", "en" %}
{% for post in posts_en %}
  <li class="post-list-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <div class="post-excerpt">{{ post.excerpt | strip_html | truncate: 180 }}</div>
    <div class="post-meta">{{ post.date | date: "%Y-%m-%d" }} • {{ post.lang }}</div>
  </li>
{% endfor %}
</ul>
