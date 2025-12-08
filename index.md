---
layout: default
title: Home
---

<header class="hero">
  <div class="hero-inner">
    <h1>Data never lie</h1>
    <p class="subtitle">Research, data science, and stories from around the world.</p>
  </div>
</header>

<section class="home-section">
  <h2>Latest posts</h2>
  <div class="post-grid">
    {% for post in site.posts limit:4 %}
      <article class="post-card">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
        <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
      </article>
    {% endfor %}
  </div>
  <p><a href="{{ '/blog' | relative_url }}" class="btn">View all posts</a></p>
</section>
