---
title: 'Letter to future: 2025-2026'
date: 2025-06-02
#permalink: /posts
categories: Letters
laout: post
#comment: true
---


Hi, <br>
I don't know the exact reason, but I feel that July is as auspicious month -- the best time of the year to start something new or reflect on the past year. Today is July 02, 2025 and I am starting this blog. I hope to write more often. Let's see where it leads. <br>
As of today, I have 3-4 posts which were written some time ago, mostly as a part of assignments or projects. I haven't changed anything; just kept them here. <br>
<br>
This is just for fun and it serves as my first post. I want to check in with myself after a year. <br> 

By  next year at this time, I will have <br>

<ul> 
<li>visited at least 3 states</li> 
<li>submitted one manuscript</li> 
<li>read 10 books, watched 20 movies, written 15 blog posts</li> <li>tried 12 new restaurants, taken 50 photos</li> 
</ul>
<ul>

I will rank myself after a year -- almost at the same time. Let's see I do


<br>
<br>
<br>
<br>
This blog appears in the category: 
<br>
 
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

