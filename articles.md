---
layout: default
title: "Articles"
permalink: /articles/
---

# 📐 System Design & Architecture Articles

<ul>
  {% for article in site.articles %}
    <li>
      <a href="{{ article.url | relative_url }}">{{ article.title }}</a>
      <small>({{ article.date | date: "%b %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>
