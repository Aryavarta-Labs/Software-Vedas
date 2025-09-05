---
layout: default
title: "Articles"
permalink: /articles/
---

# 📐 System Design & Architecture Articles

<table>
  <thead>
    <tr>
      <th>Title</th>
      <th>Categories</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    {% for article in site.articles %}
    <tr>
      <td><a href="{{ article.url | relative_url }}">{{ article.title }}</a></td>
      <td>{{ article.categories | join: ", " }}</td>
      <td>{{ article.date | date: "%b %-d, %Y" }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>



