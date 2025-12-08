---
layout: default
title: Home
---

<header class="hero">
  <div class="hero-inner">
    <p class="eyebrow">Personal website of</p>
    <h1>Elena Cuoco</h1>
    <p class="subtitle">
      Physicist, data scientist, traveller.<br>
      Exploring the universe through signals, numbers, and stories.
    </p>
    <p>
      <a href="{{ '/about' | relative_url }}" class="btn">Read my story</a>
      <a href="{{ '/research-and-academia' | relative_url }}" class="btn btn-secondary">View my research</a>
    </p>
  </div>
</header>

<section class="home-section">
  <h2>What you’ll find here</h2>

  <div class="feature-grid">
    <article class="feature-card">
      <h3>Research &amp; Academia</h3>
      <p>
        Gravitational waves, signal processing, and the joy of working in international collaborations.
        I share projects, talks, and links to papers and resources.
      </p>
      <p><a href="{{ '/research-and-academia' | relative_url }}">Dive into my research →</a></p>
    </article>

    <article class="feature-card">
      <h3>Data Science</h3>
      <p>
        From competition notebooks to real-world pipelines, I write about machine learning,
        time-series analysis, and practical tips for working with data.
      </p>
      <p><a href="{{ '/data-science' | relative_url }}">Explore data science posts →</a></p>
    </article>

    <article class="feature-card">
      <h3>Travels &amp; Photos</h3>
      <p>
        Places that inspired me, people I met, and moments I don’t want to forget —
        collected in small visual stories around the world.
      </p>
      <p><a href="{{ '/travels-and-photos' | relative_url }}">See where I’ve been →</a></p>
    </article>
  </div>
</section>

<section class="home-section">
  <h2>Latest from the blog</h2>

  {% if site.posts and site.posts.size > 0 %}
  <div class="post-grid">
    {% for post in site.posts limit:4 %}
      <article class="post-card">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
        <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
        <p><a href="{{ post.url | relative_url }}">Read more →</a></p>
      </article>
    {% endfor %}
  </div>
  <p>
    <a href="{{ '/blog' | relative_url }}" class="btn">View all posts</a>
  </p>
  {% else %}
  <p><em>No posts yet.</em> When you publish your first article in <code>_posts</code>, it will appear here.</p>
  {% endif %}
</section>

<section class="home-section home-section-alt">
  <div class="two-columns">
    <div>
      <h2>A few keywords about me</h2>
      <ul class="tag-list">
        <li>gravitational-wave astronomy</li>
        <li>signal processing</li>
        <li>machine learning</li>
        <li>Python &amp; scientific computing</li>
        <li>open science &amp; education</li>
        <li>travels &amp; photography</li>
      </ul>
    </div>
    <div>
      <h2>Elsewhere on the web</h2>
      <p>You can also find me here:</p>
      <ul>
        <li><a href="https://github.com/elenacuoco" target="_blank" rel="noopener">GitHub</a></li>
        <li><a href="https://www.linkedin.com/in/elenacuoco/" target="_blank" rel="noopener">LinkedIn</a></li>
        <li><a href="https://scholar.google.com/citations?user=kKSI7MAAAAAJ&hl=it" target="_blank" rel="noopener">Google Scholar</a></li>
        <li><a href="https://orcid.org/0000-0002-6528-3449" target="_blank" rel="noopener">ORCID</a></li>
      </ul>
    </div>
  </div>
</section>
