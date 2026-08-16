---
layout: page
title: Categories
permalink: /categories/
---

<section class="archive-shell">
  <header class="list-header">
    <p class="page-subtitle">All posts grouped by topic for quick navigation.</p>
  </header>

  <div id="archives" class="archive-grid">
  {% for category in site.categories %}
    <section class="archive-group">
      {% capture category_name %}{{ category | first }}{% endcapture %}
      <a class="archive-anchor" id="{{ category_name | slugize }}"></a>
      <h3 class="category-head">{{ category_name }} <span>({{ site.categories[category_name] | size }})</span></h3>
      {% for post in site.categories[category_name] %}
      <article class="archive-item">
        <h4><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h4>
      </article>
      {% endfor %}
    </section>
    {% endfor %}
  </div>
</section>

