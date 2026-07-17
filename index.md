---
layout: default
title: 首页
---

# 欢迎来到我的个人网站

你好！这是我的 GitHub Pages 个人网站。

## 最新文章

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <small>{{ post.date | date: "%Y年%m月%d日" }}</small>
  </li>
{% endfor %}
</ul>

## 关于我

- 💼 数字游民
- 🚗 爱好：自驾、艺术、爬山

## 项目

敬请期待更多项目展示...

---

*本站由 [GitHub Pages](https://pages.github.com/) 托管*
