---
layout: default
---

<div class="flex-row">
  <h1 style="color:blue;"> Latest blogs.... </h1>
</div>

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
      <div class="entry">
        {{ post.excerpt | strip_html | strip_newlines | truncatewords: 45 }}
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>