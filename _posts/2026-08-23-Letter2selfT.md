---
title: 'Self check -2027'
date: 2026-07-01
#permalink: /posts
categories: Letters
laout: post
#comment: true
---


Hi, <br>
This is my first post! <br>
I want to read this letter in January 2027, and reflect on the milestones I set for 2026. By then, I hope to have:
<ul> 
personally: 
<li>visited 2 new states</li>
<li>visited 1 national park or place of interest</li>
<li>tried 12 new restaurants</li>
<li>visited 1 friend's home or invited them </li>
professionally: 
<li>submitted 1 manuscript</li> 
mentally: 
<li>read 10 books, watched 20 movies</li> 
<li>written 4 new blog posts</li>
 
</ul>
<i>As this is first post and is writen in July, but it will include all activities throughout 2026. I plan to score myself based on how well I follow my plans and review it annually. </i> <br>
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

