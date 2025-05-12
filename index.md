---
layout: blog
title: Home
---

<div class="home">
  <h2>Latest Posts</h2>
  <ul class="post-list-home">
    {% for post in site.posts reversed %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</div>
