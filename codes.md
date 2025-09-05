---
layout: default
title: "Code Solutions"
permalink: /codes/
---

# 💻 Algorithms & DSA Solutions

<ul>
  {% for code in site.codes %}
    <li>
      <a href="{{ code.url | relative_url }}">{{ code.title }}</a>
      <small>({{ code.date | date: "%b %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>
