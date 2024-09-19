---
layout: page
title: "Blog"
permalink: /blog/
---
<!-- {% assign blog_posts = site.posts | where_exp: "post", "post.tags contains 'blog'" %}

{% if site.show_excerpts %}
  {% include home.html posts=blog_posts %}
{% else %}
  {% include archive.html title="Blog Posts" posts=blog_posts %}
{% endif %} -->

{% assign blog_posts = site.posts | where: "categories", "blogs" %}

{% if site.show_excerpts %}
  {% include home.html posts=blog_posts %}
{% else %}
  {% include archive.html title="Blog Posts" posts=blog_posts %}
{% endif %}

<!-- - [1. Hello World](_posts/2024-09-19-blog-1.md) -->