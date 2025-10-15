---
layout: default
title: "ქართული"
permalink: /ge/
---
# ქართულად

<ul class="post-list">
{% assign posts_ge = site.posts | where: "lang", "ge" %}
{% for post in posts_ge %}
  <li class="post-list-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <div class="post-excerpt">{{ post.excerpt | strip_html | truncate: 180 }}</div>
    <div class="post-meta">{{ post.date | date: "%Y-%m-%d" }} • {{ post.lang }}</div>
  </li>
{% endfor %}
</ul>

