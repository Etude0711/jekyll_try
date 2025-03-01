---
layout: default
title: 首页
---

# 欢迎来到我的Jekyll网站

这是一个使用Jekyll创建的简单网站，专为GitHub Pages设计。

## 最新文章

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h2>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h2>
      <p class="post-meta">
        {{ post.date | date: "%Y年%m月%d日" }}
        {% if post.categories %}
        • 
        <span class="post-categories">
          分类：
          {% for category in post.categories %}
            <span class="post-category">{{ category }}</span>
          {% endfor %}
        </span>
        {% endif %}
      </p>
      <p>
        {{ post.excerpt }}
      </p>
      <a href="{{ post.url | relative_url }}">阅读全文 &raquo;</a>
    </li>
  {% endfor %}
</ul>
