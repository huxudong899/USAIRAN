# 🇺🇸 🇮🇷 USAIRAN - 美伊战况每日简报

> **自动追踪** · **每日更新** · **多源聚合** · **AI驱动**

[🌐 访问网站](https://huxudong899.github.io/USAIRAN/)

---

## 🎯 项目简介

**USAIRAN** 是一个基于 GitHub Pages 的自动化新闻发布系统，专门追踪美伊战争相关新闻。系统由 **OpenClaw AI Agent** 驱动，每天自动从全球主流媒体聚合最新报道，生成结构化的新闻简报。

✨ **全新 v2.0 版本已上线！** 采用现代化卡片式设计，响应式布局，提供极致的阅读体验。

---

## 🌟 核心特性

- 🎨 **现代化设计** - 渐变主题、卡片布局、流畅动画
- 📱 **完美响应式** - 手机、平板、桌面全覆盖
- 🤖 **AI自动化** - 自动搜索、提取、发布，无需人工干预
- 📊 **智能统计** - 实时展示简报数量、更新状态
- 🔖 **分类归档** - 按日期浏览完整历史
- ⚡ **极速加载** - 纯静态页面，GitHub Pages CDN 全球分发

---

## 📺 在线访问

### 首页
[https://huxudong899.github.io/USAIRAN/](https://huxudong899.github.io/USAIRAN/)

### 历史存档
[https://huxudong899.github.io/USAIRAN/archive/](https://huxudong899.github.io/USAIRAN/archive/)

---

## 🗞️ 最新简报

{% for post in site.posts limit:3 %}
- **[{{ post.date | date: "%Y-%m-%d" }}]({{ post.url | relative_url }})** - {{ post.title | replace: "美伊战况简报 - ", "" }}
{% endfor %}

查看 [📋 完整历史存档](archive/) 获取所有过往简报。

---

## ⚙️ 技术架构

| 组件 | 技术 | 描述 |
|------|------|------|
| **前端框架** | Jekyll + Liquid | 静态站点生成 |
| **样式** | CSS3 + Custom Properties | 现代渐变、动画、响应式 |
| **托管平台** | GitHub Pages | 免费、全球CDN、自动HTTPS |
| **CI/CD** | GitHub Actions | 自动构建部署 |
| **自动化引擎** | OpenClaw | AI Agent 自动执行搜索、抓取、发布 |
| **数据源** | Google News, BBC, Reuters, 新华网, 人民网等 | 多源聚合 |

---

## 🚀 快速部署

想部署自己的自动化新闻系统？只需 5 步：

```bash
# 1. Fork 本仓库
# 2. 复制 iran-news-publisher.yaml 到你的 OpenClaw 配置
# 3. 修改搜索关键词和发布目标
# 4. 配置 GitHub Personal Access Token
# 5. 启用定时任务，坐等自动推送
```

详细配置说明：
- 编辑 `iran-news-publisher.yaml` 调整搜索参数
- 修改 `_config.yml` 更新网站标题、描述等元信息
- 在 GitHub 仓库设置中添加 `GITHUB_TOKEN` Secret

---

## 📁 项目结构

```
USAIRAN/
├── _config.yml          # Jekyll 配置
├── index.html           # 首页（现代化设计）
├── archive.html         # 归档页面
├── _layouts/
│   └── default.html    # 全局布局模板
├── _includes/
│   ├── header.html     # 页头
│   └── footer.html     # 页脚
├── assets/
│   └── css/
│       └── style.css   # 样式表（v2.0 全新设计）
├── news/               # 新闻 Markdown 文件
│   ├── 2025-03-20.md
│   ├── 2025-03-21.md
│   └── 2025-03-22.md
└── README.md           # 本文件
```

---

## 🎨 样式特性

- ✨ **渐变英雄区域** - 顶部大横幅配合动态背景图案
- 🎴 **卡片式布局** - 悬停动画 + 顶部渐变条
- 📊 **统计展示** - 醒目的大数字显示
- 🖱️ **微交互** - 所有可点击元素都有过渡动画
- 🎯 **无障碍** - 语义化 HTML，ARIA 标签支持
- 🎭 **暗色模式就绪** - CSS 变量，易于切换主题

---

## 🤝 贡献

欢迎提 Issue 和 Pull Request！

如果你想：
- 改进新闻抓取逻辑
- 增加新的新闻源
- 优化 UI/UX 设计
- 添加新功能（订阅、RSS 等）

请先 fork 本仓库，然后提交 PR。

---

## ⚠️ 免责声明

本网站内容**仅供研究与学习参考**，不代表任何官方立场。所有新闻内容来源于公开媒体，版权归原作者所有。如有疑问请参考原始来源。

---

## 📬 联系方式

- **技术栈**: OpenClaw AI Agent Framework
- **文档**: https://docs.openclaw.ai
- **仓库**: https://github.com/huxudong899/USAIRAN

---

<div align="center">

**Built with ❤️ by OpenClaw**

 Made with Jekyll • Hosted on GitHub Pages

</div>
