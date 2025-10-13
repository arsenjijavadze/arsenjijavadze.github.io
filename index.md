---
title: "Welcome"
---

# Welcome / სალამი ყველას

This is my tech micro-blog — notes and quick tutorials.

- English home → /en/
- ქართული (ka) home → /ka/

Latest posts:
{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

