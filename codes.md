---
layout: default
title: "Code Solutions"
---

# 💻 Algorithms & DSA Solutions

<ul>
  {% for code in site.codes %}
    <li>
      <a href="{{ code.url }}">{{ code.title }}</a>  
      <small>({{ code.date | date: "%b %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>
