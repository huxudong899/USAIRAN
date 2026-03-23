---
layout: default
title: 调试页面
permalink: /debug/
---

# Debug Info

- **site.posts 数量**: {{ site.posts | size }}
- **site.pages 数量**: {{ site.pages | size }}
- **site.static_files 数量**: {{ site.static_files | size }}

{% comment %}
First 3 posts:
{% for post in site.posts limit:3 %}
  - {{ post.date }}: {{ post.title }} (url: {{ post.url }})
{% endfor %}
{% endcomment %}
