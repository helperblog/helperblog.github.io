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

  {% if site.posts.size > 3 %}
  <div class="popular-posts">
    <h2>Popular Posts (Newest First)</h2>
    <ul class="post-list-home">
      {% for post in site.posts limit:3 reversed %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
        </li>
      {% endfor %}
    </ul>
  </div>
  {% endif %}
</div>
