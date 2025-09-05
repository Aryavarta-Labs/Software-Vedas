---
layout: default
title: "Posts"
permalink: /posts/
---

# 📝 Posts  
Daily updates on my corporate life, conferences, and hackathons.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>  
      <small>({{ post.date | date: "%b %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>
