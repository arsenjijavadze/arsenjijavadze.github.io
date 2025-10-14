---
layout: default
title: Home
---

# Welcome

Hi, I’m **Arsen** — a software engineer exploring development, DevOps, and systems.

Here you’ll find short notes, practical how-tos, and reflections about technology, engineering, and continuous learning.

---

## Latest posts

<ul class="post-list">
{% for post in site.posts %}
  <li class="post-list-item">
    <a href="{{ post.url | relative_url }}">
      <strong>{{ post.title }}</strong>
    </a>
    <div class="post-excerpt">
      {{ post.excerpt | strip_html | truncate: 180 }}
    </div>
    <div class="post-meta">
      {{ post.date | date: "%Y-%m-%d" }} • {% if post.tags %}{{ post.tags | join: ", " }}{% endif %}
    </div>
  </li>
{% endfor %}
</ul>
