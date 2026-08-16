---
layout: default
---

<hr style="height:1px;border-width:0;color:gray;background-color:GhostWhite">

<br>

<div class="flex-row">
  <h1 style="color:blue;"> Latest blogs.... </h1>
</div>

<!-- code that will arrange the blogs according to the date -->

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
      <div class="entry">
        {{ post.excerpt }}
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>