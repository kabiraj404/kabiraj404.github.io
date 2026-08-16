---
title: 'Letter to future -2027'
date: 2026-01-15
#permalink: /posts
categories: Letters
laout: post
#comment: true
---


Hi, <br>
This is my first post! I want to check in with myself in a year. <br> 
By  next year at this time, I will have:
<ul> 
<li>visited at least 2 states</li> 
<li>submitted one manuscript</li> 
<li>read 10 books, watched 20 movies</li> 
<li>written 15 blog posts</li> 
<li>tried 12 new restaurants</li> 
</ul>
I will rank myself after a year -- almost at the same time. <br>
Happy new year 2026! 
<br>
<br>
<br>
<br>
<i style="color: #bf7039">This blog appears in the category: </i>
<div class="post-categories">
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
  <a href="{{site.baseurl}}/categories/#{{category|slugize}}">{{category}}</a>
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>

