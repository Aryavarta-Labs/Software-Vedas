---
layout: default
title: "Home"
---

<!-- 🎯 Hero Section -->
<div style="text-align: center; padding: 3rem 1rem; background: #f4f4f4; border-radius: 12px; margin-bottom: 2rem;">
  <h1 style="font-size: clamp(2rem, 5vw, 2.8rem); margin-bottom: 0.5rem;">🕉️ Software Vedas</h1>
  <p style="font-size: clamp(1rem, 2.5vw, 1.2rem); color: #444; max-width: 700px; margin: auto;">
    <b>The Gita Saar of all Software Wisdom</b> curated in four bricks — <b>Posts</b>, <b>Products</b>, <b>Articles</b>, and <b>Codes</b>.
  </p>
</div>

---

## 📑 Explore Knowledge
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem; margin-bottom: 2rem;">

  <a href="{{ site.baseurl }}/posts/" style="padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit; display: block;">
    <h2>📝 Posts</h2>
    <p>Daily updates from my corporate life, conferences & hackathons.</p>
  </a>

  <a href="{{ site.baseurl }}/products/" style="padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit; display: block;">
    <h2>📦 Products</h2>
    <p>Documentation of MVPs I built during hackathons.</p>
  </a>

  <a href="{{ site.baseurl }}/articles/" style="padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit; display: block;">
    <h2>📘 Articles</h2>
    <p>Literature for developers on system design, architecture, and software product lifecycle.</p>
  </a>

  <a href="{{ site.baseurl }}/codes/" style="padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit; display: block;">
    <h2>💻 Codes</h2>
    <p>Code snippets to learn data structures, algorithms, and programming languages.</p>
  </a>

</div>

---

## 🆕 Latest Updates
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem;">

  <!-- Posts -->
  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>📝 Recent Posts</h3>
    <ul>
      {% for post in site.posts limit:5 %}
        <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
    <a href="{{ site.baseurl }}/posts/" style="font-weight: bold; text-decoration: none;">+ More…</a>
  </div>

  <!-- Products -->
  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>📦 Recent Products</h3>
    <ul>
      {% for product in site.products limit:5 %}
        <li><a href="{{ product.url | relative_url }}">{{ product.title }}</a></li>
      {% endfor %}
    </ul>
    <a href="{{ site.baseurl }}/products/" style="font-weight: bold; text-decoration: none;">+ More…</a>
  </div>

  <!-- Articles -->
  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>📘 Recent Articles</h3>
    <ul>
      {% for article in site.articles limit:5 %}
        <li><a href="{{ article.url | relative_url }}">{{ article.title }}</a></li>
      {% endfor %}
    </ul>
    <a href="{{ site.baseurl }}/articles/" style="font-weight: bold; text-decoration: none;">+ More…</a>
  </div>

  <!-- Codes -->
  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>💻 Recent Codes</h3>
    <ul>
      {% for code in site.codes limit:5 %}
        <li><a href="{{ code.url | relative_url }}">{{ code.title }}</a></li>
      {% endfor %}
    </ul>
    <a href="{{ site.baseurl }}/codes/" style="font-weight: bold; text-decoration: none;">+ More…</a>
  </div>

</div>

---

## 🌐 Connect with Me
<div style="text-align: center; margin-top: 2rem;">

  <p style="margin-bottom: 1rem;">Let’s connect and grow together 🚀</p>

  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 0.5rem;">
    <a href="https://www.linkedin.com/company/aryavarta-labs/" target="_blank"
       style="flex: 1 1 200px; text-align: center; padding: 0.8rem; background: #0077b5; color: white; font-weight: bold; text-decoration: none; border-radius: 6px;">
      💼 Follow on LinkedIn
    </a>
    <a href="https://github.com/Aryavarta-Labs" target="_blank"
       style="flex: 1 1 200px; text-align: center; padding: 0.8rem; background: #fbbc05; color: black; font-weight: bold; text-decoration: none; border-radius: 6px;">
      ⭐ Follow on Github
    </a>
  </div>
</div>
