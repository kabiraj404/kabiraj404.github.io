---
layout: page
title: Categorized blogs 
permalink: /categories/
---



#### All of the blogs are listed here, organized by category. Please click <a class="break-long-url" target="_blank" href="https://kabiraj404.github.io/blog/">HERE</a> to return to the home page. 

<hr style="height:1px;border-width:0;color:gray;background-color:GhostWhite">


<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>

