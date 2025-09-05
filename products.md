---
layout: default
title: "Products"
permalink: /products/
---

# 📝 Product Development Posts

<ul>
  {% for product in site.products %}
    <li>
      <a href="{{ product.url | relative_url }}">{{ product.title }}</a>
      <small>({{ product.date | date: "%b %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>
