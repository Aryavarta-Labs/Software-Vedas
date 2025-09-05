---
layout: default
title: "Software Vedas"
---

<!-- 🎯 Hero Section -->
<div style="text-align: center; padding: 3rem 1rem; background: #f4f4f4; border-radius: 12px; margin-bottom: 2rem;">
  <h1 style="font-size: 2.5rem; margin-bottom: 0.5rem;">🕉️ Software Vedas</h1>
  <p style="font-size: 1.2rem; color: #444; max-width: 700px; margin: auto;">
    <b>The Gita Saar of all Software Wisdom</b> curated in four bricks — <b>Posts</b>, <b>Products</b>, <b>Articles</b>, and <b>Codes</b>.
  </p>
</div>

---

## 📑 Explore Knowledge
<div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem; margin-bottom: 2rem;">

  <a href="{{ site.baseurl }}/posts/" style="flex: 1 1 250px; padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit;">
    <h2>📝 Posts</h2>
    <p>Daily updates from my corporate life, <br> conferences & hackathons.</p>
  </a>

  <a href="{{ site.baseurl }}/products/" style="flex: 1 1 250px; padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit;">
    <h2>📦 Products</h2>
    <p>Documentation of MVPs <br> I built during hackathons.</p>
  </a>

  <a href="{{ site.baseurl }}/articles/" style="flex: 1 1 250px; padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit;">
    <h2>📘 Articles</h2>
    <p>Literature for developers on <br> system design, architecture, and <br> software product lifecycle.</p>
  </a>

  <a href="{{ site.baseurl }}/codes/" style="flex: 1 1 250px; padding: 1.2rem; background: #fff; border-radius: 12px; box-shadow: 0 2px 6px rgba(0,0,0,0.1); text-decoration: none; color: inherit;">
    <h2>💻 Codes</h2>
    <p>Code snippets to learn <br> data structures, algorithms, <br> and programming languages.</p>
  </a>

</div>

---

## 🆕 Latest Updates

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem;">

  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>📝 Recent Posts</h3>
    <ul>
      {% for post in site.posts limit:5 %}
        <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </div>

  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>📦 Recent Products</h3>
    <ul>
      {% for product in site.products limit:5 %}
        <li><a href="{{ product.url | relative_url }}">{{ product.title }}</a></li>
      {% endfor %}
    </ul>
  </div>

  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>📘 Recent Articles</h3>
    <ul>
      {% for article in site.articles limit:5 %}
        <li><a href="{{ article.url | relative_url }}">{{ article.title }}</a></li>
      {% endfor %}
    </ul>
  </div>

  <div style="background: #fff; padding: 1rem; border-radius: 8px; box-shadow: 0 1px 4px rgba(0,0,0,0.08);">
    <h3>💻 Recent Codes</h3>
    <ul>
      {% for code in site.codes limit:5 %}
        <li><a href="{{ code.url | relative_url }}">{{ code.title }}</a></li>
      {% endfor %}
    </ul>
  </div>

</div>

---

## 🌐 Connect with Me

<div style="text-align: center; margin-top: 2rem;">
  <p>Let’s connect and grow together 🚀</p>

  <a href="https://topmate.io/erakashsrivastava" target="_blank"
     style="padding: 0.6rem 1.2rem; background: #6c63ff; color: white; font-weight: bold; text-decoration: none; border-radius: 6px; margin: 0.3rem; display: inline-block;">
    🎙️ Connect on Topmate
  </a>

  <a href="https://www.linkedin.com/in/akash-srivastava-public/" target="_blank"
     style="padding: 0.6rem 1.2rem; background: #0077b5; color: white; font-weight: bold; text-decoration: none; border-radius: 6px; margin: 0.3rem; display: inline-block;">
    💼 Follow on LinkedIn
  </a>

  <a href="https://www.youtube.com/@er.akash.srivastava" target="_blank"
     style="padding: 0.6rem 1.2rem; background: #ff0000; color: white; font-weight: bold; text-decoration: none; border-radius: 6px; margin: 0.3rem; display: inline-block;">
    ▶️ Subscribe on YouTube
  </a>
</div>
