---
layout: default
title: Home
---

# Nishant Modak

Software engineer and entrepreneur based in California.

## Recent Posts

<div class="post-card-container">
  {% for post in site.posts limit:3 %}
    <div class="post-card">
      {% if post.image %}
        <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="post-card-image">
      {% else %}
        <div class="post-card-image-placeholder"></div>
      {% endif %}
      <div class="post-card-content">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      </div>
    </div>
  {% endfor %}
</div>

[All posts](/blog)

## Projects

- [Project One](link-to-project-one) - Brief description
- [Project Two](link-to-project-two) - Brief description
- [Project Three](link-to-project-three) - Brief description

[All projects](/projects)