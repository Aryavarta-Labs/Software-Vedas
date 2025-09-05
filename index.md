---
layout: default
title: "Software Vedas"
---

# 🕉️ Software Vedas

Welcome to **Software Vedas** — Insights on **Product Development**, **System Design & Architecture**, and **DSA/Algorithms**.

---

## 📑 Navigation
<nav style="margin: 1rem 0; font-size: 1.2rem; font-weight: bold;">
  <a href="{{ site.baseurl }}/posts/" style="margin-right: 1rem;">📝 Posts</a>
  <a href="{{ site.baseurl }}/articles/" style="margin-right: 1rem;">📘 Articles</a>
  <a href="{{ site.baseurl }}/codes/" style="margin-right: 1rem;">💻 Codes</a>
  <a href="{{ site.baseurl }}/products/" style="margin-right: 1rem;">📦 Products</a>
</nav>

---

## 🆕 Latest Updates

### 📝 Posts
<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> — 
      <small>{{ post.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

### 📘 Articles
<ul>
  {% for article in site.articles limit:5 %}
    <li>
      <a href="{{ article.url | relative_url }}">{{ article.title }}</a> — 
      <small>{{ article.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

### 💻 Codes
<ul>
  {% for code in site.codes limit:5 %}
    <li>
      <a href="{{ code.url | relative_url }}">{{ code.title }}</a> — 
      <small>{{ code.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

### 📦 Products
<ul>
  {% for product in site.products limit:5 %}
    <li>
      <a href="{{ product.url | relative_url }}">{{ product.title }}</a> — 
      <small>{{ product.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

---

## 📡 Subscribe

<div class="subscribe-box">
  <h2>📡 Stay Updated</h2>
  <p>Follow the latest Articles, Posts, Codes, and Products.</p>

  <!-- Direct RSS Feed -->
  <a href="{{ '/feed.xml' | relative_url }}" target="_blank"
     style="padding: 0.6rem 1.2rem; 
            background: #ff6600; 
            color: white; 
            font-weight: bold; 
            text-decoration: none; 
            border-radius: 6px; 
            margin: 0.3rem;
            display: inline-block;">
    📩 RSS Feed (XML)
  </a>

  <!-- Feedly Button -->
  <a href="https://feedly.com/i/subscription/feed/{{ site.url }}{{ site.baseurl }}/feed.xml" target="_blank"
     style="padding: 0.6rem 1.2rem; 
            background: #2bb24c; 
            color: white; 
            font-weight: bold; 
            text-decoration: none; 
            border-radius: 6px; 
            margin: 0.3rem;
            display: inline-block;">
    📰 Subscribe in Feedly
  </a>
</div>
