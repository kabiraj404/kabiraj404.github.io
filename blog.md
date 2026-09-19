---
layout: default
title: Blog
permalink: /blog/
---

<section class="listing-shell">
  <header class="list-header">
    <h1 class="page-title">Latest blogs</h1>
    <div class="blog-hub-links" aria-label="Blog hub links">
      <a href="{{ site.baseurl }}/feed.xml">RSS</a>
    </div>
  </header>

  <div class="posts post-list">
  {% for post in site.posts %}
    <article class="post post-card">
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
            <small class="post-list-date">{{ post.date | date: "%b %e, %Y" }}</small></h2> 
      <div class="entry post-excerpt">
        {{ post.excerpt | strip_html | strip_newlines | truncatewords: 20 }}
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
        </div>
    </article>
  {% endfor %}
  </div>
</section>