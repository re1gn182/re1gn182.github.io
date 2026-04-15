---
layout: default
title: Home
---

<section class="hero">
  <p class="eyebrow">re1gn</p>
  <h1>Notes, builds, and writeups.</h1>
  <p class="lead">
    A personal blog for projects, cybersecurity work, Linux experiments, and whatever else I’m building.
  </p>
  <div class="hero-actions">
    <a class="button" href="{{ '/about' | relative_url }}">About Me</a>
    <a class="button button-ghost" href="{{ '/projects' | relative_url }}">See Projects</a>
  </div>
</section>

<section class="card-section">
  <div class="section-head">
    <h2>Latest posts</h2>
    <p>Markdown posts in <code>_posts</code>.</p>
  </div>

  <div class="post-list">
    {% assign posts_count = site.posts | size %}
    {% if posts_count > 0 %}
      {% for post in site.posts limit: 6 %}
        <a class="post-card" href="{{ post.url | relative_url }}">
          <p class="meta">{{ post.date | date: "%b %-d, %Y" }}</p>
          <h3>{{ post.title }}</h3>
          <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
        </a>
      {% endfor %}
    {% else %}
      <div class="post-card">
        <p class="meta">No posts yet</p>
        <h3>Start writing</h3>
        <p>Create a new Markdown file in <code>_posts</code> and Jekyll will handle the rest.</p>
      </div>
    {% endif %}
  </div>
</section>
