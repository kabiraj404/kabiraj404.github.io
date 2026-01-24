---
layout: page
#title: Categorized blogs 
permalink: /categories/
---



#### All blogs are listed here, organized by category.  

<hr style="height:1px;border-width:0;color:gray;background-color:GhostWhite">


<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    <ul style="padding-left: 20px;">
      {% for post in site.categories[category_name] %}
      <li class="archive-item">
        <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
      </li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}
</div>

