---
layout: default
title: Blog
permalink: /blog/
---

# Blog Posts

Welcome to my blog! Here you'll find my thoughts, experiences, and insights on [main topics you'll write about].

{% for post in site.posts %}
  <article class="post-preview">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-meta">
      {{ post.date | date: "%B %d, %Y" }}
      {% if post.tags.size > 0 %}
        <span class="post-tags">
          {% for tag in post.tags %}
            <span class="tag">{{ tag }}</span>
          {% endfor %}
        </span>
      {% endif %}
    </p>
    {{ post.excerpt }}
  </article>
{% endfor %}