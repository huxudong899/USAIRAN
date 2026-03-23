---
layout: none
title: 历史存档
permalink: /archive/
---

# 历史存档 (测试版)

<p>📊 site.posts 数量: {{ site.posts | size }}</p>

{% comment %} 开始循环 {% endcomment %}
{% for post in site.posts %}
<p>🔹 {{ post.date | date: "%Y-%m-%d" }} - <a href="{{ post.url | relative_url }}">{{ post.title }}</a></p>
{% endfor %}

{% if site.posts.size == 0 %}
<p>⚠️ site.posts 为空！请检查 _posts 目录。</p>
{% endif %}
