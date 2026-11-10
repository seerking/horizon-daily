---
layout: default
title: Horizon Daily
---

# 🌅 Horizon Daily

AI 精选的每日科技简报 —— Hacker News、RSS、Reddit、GitHub 多源采集，DeepSeek 打分去重，每条带背景、实用影响与社区讨论。

## 每日简报

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.date | date: "%Y-%m-%d" }}</a> — {{ post.title }}
    </li>
  {% else %}
    <li><em>暂无内容</em></li>
  {% endfor %}
</ul>

## 说明

- 每天北京时间早上自动更新
- 生成器：[Horizon](https://github.com/Thysrael/Horizon)（MIT）
- 自动任务：Hermes Agent · 模型 DeepSeek
