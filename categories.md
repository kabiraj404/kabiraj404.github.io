---
layout: page
permalink: /categories/
---

<header class="category-index-header">
  <p class="subtitle">All posts grouped by topic.</p>
</header>

<div class="category-grid">
  {% assign sorted_categories = site.categories | sort %}
  {% for category in sorted_categories %}
    {% assign category_name = category | first %}
    {% assign category_posts = category | last %}
    
    <section id="{{ category_name | slugify }}" class="category-group">
      <div class="category-meta">
        <h2 class="category-title">{{ category_name }}</h2>
      </div>

      <ul class="category-posts">
        {% for post in category_posts %}
          <li class="post-row">
            <time class="post-date" datetime="{{ post.date | date_to_xmlschema }}">
              {{ post.date | date: "%Y, %d %b" }}
            <a href="{{ post.url | relative_url }}" class="post-link">{{ post.title }}</a>
            </time>
          </li>
        {% endfor %}
      </ul>
    </section>
  {% endfor %}
</div>