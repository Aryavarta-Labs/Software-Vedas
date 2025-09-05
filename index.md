---
layout: default
title: "Software Vedas"
---

<style>
/* 🔹 Tabs */
.tab-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  margin: 1rem 0;
}
.tab {
  padding: 0.6rem 1.2rem;
  cursor: pointer;
  border: 1px solid #ddd;
  border-radius: 8px 8px 0 0;
  margin: 0.2rem;
  background: #f9f9f9;
  font-weight: bold;
  transition: all 0.3s ease;
}
.tab.active {
  background: #0366d6;
  color: white;
  border-bottom: 2px solid white;
}
.tab:hover {
  background: #e6e6e6;
}

/* 🔹 Content Sections */
.tab-content {
  display: none;
  padding: 1rem;
  border: 1px solid #ddd;
  border-radius: 0 8px 8px 8px;
  background: white;
  max-height: 300px;
  overflow-y: auto;
}
.tab-content.active {
  display: block;
}

/* 🔹 Post List */
.post-item {
  margin-bottom: 1rem;
}
.post-item a {
  text-decoration: none;
  color: #0366d6;
  font-weight: 600;
}
.post-item small {
  color: #888;
}

/* 🔹 Subscribe Section */
.subscribe-box {
  text-align: center;
  margin: 2rem 0;
  padding: 1.5rem;
  border: 1px solid #ddd;
  border-radius: 10px;
  background: #f8faff;
}
.subscribe-box a {
  display: inline-block;
  margin-top: 0.8rem;
  padding: 0.6rem 1.2rem;
  background: #ff6600;
  color: white;
  font-weight: bold;
  text-decoration: none;
  border-radius: 6px;
  transition: background 0.3s ease;
}
.subscribe-box a:hover {
  background: #cc5200;
}
</style>

<div style="text-align: center; padding: 1rem;">
  <h1>🕉️ Software Vedas</h1>
  <p><i>Insights on Product Development, System Design, and DSA</i></p>
</div>

<!-- 🔹 Tabs -->
<div class="tab-container">
  <div class="tab active" onclick="showTab('posts')">📝 Posts</div>
  <div class="tab" onclick="showTab('articles')">📐 Articles</div>
  <div class="tab" onclick="showTab('codes')">💻 Codes</div>
  <div class="tab" onclick="showTab('products')">🛠 Products</div>
</div>

<!-- 🔹 Tab Contents -->
<div id="posts" class="tab-content active">
  <h2>Latest Posts</h2>
  <ul>
    {% for post in site.posts limit:5 %}
      <li class="post-item">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small>({{ post.date | date: "%b %d, %Y" }})</small>
      </li>
    {% endfor %}
  </ul>
  <p><a href="{{ '/posts/' | relative_url }}">See all posts →</a></p>
</div>

<div id="articles" class="tab-content">
  <h2>Latest Articles</h2>
  <ul>
    {% for article in site.articles limit:5 %}
      <li class="post-item">
        <a href="{{ article.url | relative_url }}">{{ article.title }}</a>
        <small>({{ article.date | date: "%b %d, %Y" }})</small>
      </li>
    {% endfor %}
  </ul>
  <p><a href="{{ '/articles/' | relative_url }}">See all articles →</a></p>
</div>

<div id="codes" class="tab-content">
  <h2>Latest Code Solutions</h2>
  <ul>
    {% for code in site.codes limit:5 %}
      <li class="post-item">
        <a href="{{ code.url | relative_url }}">{{ code.title }}</a>
        <small>({{ code.date | date: "%b %d, %Y" }})</small>
      </li>
    {% endfor %}
  </ul>
  <p><a href="{{ '/codes/' | relative_url }}">See all codes →</a></p>
</div>

<div id="products" class="tab-content">
  <h2>Latest Product Insights</h2>
  <ul>
    {% for product in site.products limit:5 %}
      <li class="post-item">
        <a href="{{ product.url | relative_url }}">{{ product.title }}</a>
        <small>({{ product.date | date: "%b %d, %Y" }})</small>
      </li>
    {% endfor %}
  </ul>
  <p><a href="{{ '/products/' | relative_url }}">See all products →</a></p>
</div>

<!-- 🔹 Subscribe Box -->
<div class="subscribe-box">
  <h2>📡 Subscribe</h2>
  <p>Follow the latest articles, posts, codes, and products via RSS.</p>
  <a href="{{ '/feed.xml' | relative_url }}">📩 Subscribe via RSS</a>
</div>

<script>
function showTab(tabId) {
  document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
  document.querySelectorAll('.tab-content').forEach(c => c.classList.remove('active'));
  document.getElementById(tabId).classList.add('active');
  event.target.classList.add('active');
}
</script>
