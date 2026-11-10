---
layout: default
title: Horizon 每日科技简报
---

## 每日简报

<ul>
  {% for post in site.posts %}
    <li><a href="{{ post.url | relative_url }}">{{ post.date | date: "%Y-%m-%d" }}</a> · {{ post.title }}</li>
  {% else %}
    <li><em>暂无内容</em></li>
  {% endfor %}
</ul>

## 关于

多源抓取（Hacker News / RSS / Reddit / GitHub）→ DeepSeek 打分去重 → 每条附背景、实用影响、社区讨论。

- 生成器：[Horizon](https://github.com/Thysrael/Horizon)（MIT）
- 流水线：Hermes Agent，手工触发
