---
layout: default
title: "Articles"
permalink: /articles/
---

# 📐 System Design & Architecture Articles

| Title                                       | Categories           | Date       |
|---------------------------------------------|--------------------|------------|
{% for article in site.articles %}
| [{{ article.title }}]({{ article.url | relative_url }}) | {{ article.categories | join: ", " }} | {{ article.date | date: "%b %-d, %Y" }} |
{% endfor %}


