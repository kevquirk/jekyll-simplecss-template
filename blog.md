---
layout: default
title: My blog
description: This is my blog, you can change this description in the front matter of blog.md
image: /assets/images/simple-css-feature.webp
---

{% for post in site.posts %}
  <div class="blog-item">
    <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
    <p class="meta"><i>{{ post.description }}</i></p>
    <p class="meta">{{ post.date | date_to_string }}</p>
  </div>
{% endfor %}
