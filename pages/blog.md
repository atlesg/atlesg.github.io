---
layout: page
title: "Blog"
permalink: /blog/
---
{% assign blog_posts = site.posts | where: "categories", "blog" %}

{% if site.show_excerpts %}
  {% include home.html posts=blog_posts %}
{% else %}
  {% include archive.html title="Some random writings..." posts=blog_posts %}
{% endif %}

<!-- - [1. Hello World](_posts/2024-09-19-blog-1.md) -->