---
layout: default
title: Home
---

# Nishant Modak

Software engineer and entrepreneur based in [Your Location].

## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[All posts](/blog)

## Projects

- [Project One](link-to-project) - Brief description
- [Project Two](link-to-project) - Brief description
- [Project Three](link-to-project) - Brief description

[All projects](/projects)