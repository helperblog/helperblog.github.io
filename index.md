---
layout: default
title: Home
description: Helper Blog - Your go-to place for clear and simple tech tutorials.
---

<section class="text-center my-5">
  <h1>Welcome to Helper Blog</h1>
  <p class="lead">Your ultimate guide for tech tutorials, tips, and how-to guides.</p>
</section>

<section>
  <h2>Latest Tutorials</h2>
  <ul class="list-group">
    {% for post in site.posts limit:5 %}
      <li class="list-group-item">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</section>

