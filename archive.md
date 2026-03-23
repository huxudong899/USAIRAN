---
layout: default
title: 历史存档
permalink: /archive/
---

# 历史存档

{% assign posts_count = site.posts | size %}
<p>📊 共 {{ posts_count }} 篇简报</p>

<ul class="archive-list">
{% for post in site.posts %}
  <li class="archive-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="archive-date">{{ post.date | date: "%Y年%m月%d日" }}</span>
    <small style="color: #999;">({{ post.url | relative_url }})</small>
  </li>
{% endfor %}
</ul>
