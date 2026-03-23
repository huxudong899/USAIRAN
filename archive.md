---
layout: default
title: 历史存档
permalink: /archive/
---

# 📜 历史存档

{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
<p>📊 共 <strong>{{ sorted_posts.size }}</strong> 篇简报</p>

<ul class="archive-list">
{% for post in sorted_posts %}
  <li class="archive-item">
    <div>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <div style="margin-top: 4px; font-size: 0.85rem; color: var(--text-light);">
        📅 {{ post.date | date: "%Y年%m月%d日" }}
        &nbsp;|&nbsp;
        🔗 <code style="background: rgba(0,0,0,0.05); padding: 2px 6px; border-radius: 4px;">{{ post.url | relative_url }}</code>
      </div>
    </div>
  </li>
{% endfor %}
</ul>

<style>
.archive-list { list-style: none; padding: 0; }
.archive-item {
  padding: 16px 20px;
  background: var(--bg-secondary);
  margin-bottom: 10px;
  border-radius: 8px;
  border-left: 4px solid var(--primary-color);
  transition: all 0.2s;
}
.archive-item:hover {
  border-left-color: var(--secondary-color);
  transform: translateX(4px);
}
.archive-item a {
  color: var(--text-primary);
  text-decoration: none;
  font-weight: 600;
  font-size: 1.05rem;
}
.archive-item a:hover {
  color: var(--primary-color);
}
.archive-item code {
  font-family: ui-monospace, SFMono-Regular, "SF Mono", Menlo, Consolas, monospace;
  font-size: 0.8rem;
}
</style>