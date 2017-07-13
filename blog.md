---
layout: page
permalink: /blog/
title: blog
description: Description here
order: 4
---

<div class="header-bar">
  <h1>Blog</h1>
  <h2>thoughts I'd like to share</h2>
  <br/>
  <hr>
  <br/>
</div>


<ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ post.description }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>
