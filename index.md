---
layout: home
title: Welcome
---

# Welcome to My Personal Site

Hello! I'm Nishant Modak, a [your profession/role] based in [your location].

This site serves as a hub for my thoughts, projects, and professional journey. Here's what you can find:

- [Blog](/blog): My latest articles and insights on [main topics].
- [Projects](/projects): Showcase of my work and contributions.
- [About Me](/about): Learn more about my background and expertise.

Feel free to explore and get in touch if you'd like to connect or collaborate!

## Recent Blog Posts

{% for post in site.posts limit:3 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.excerpt }}</p>
{% endfor %}

[View all posts](/blog)
