---
title: 'broken pieces from cozy bookmark '
date: 2026-09-01
#permalink: /posts
categories: Tiny_projects
laout: post
#comment: true
---

<br>
[Here is my reading list](https://kabiraj404.github.io/ReadingList/) 
<br>
I try to bookmark interesting articles in this collection, but some websites prevent my bookmarking tool from saving their data. I am happy with my overall bookmarking setup, so I don't want to change it just to add some of few addional websites in the list. However, when I come across notable reads, I will do my best to share them here on this blog. 
Here are a few that I found interesting recently:

1. [That’s Not How Email Works, HSBC ](https://danq.me/2026/01/28/hsbc-dont-understand-email/) 1/29/2026
2. https://www.nationalgeographic.com/culture/article/japanese-jazz-kissa-cafe (2/6/2026)
3. https://www.nationalgeographic.com/travel/article/american-towns-taste-of-scandinavia (2/6/2026)
4. https://maggieappleton.com/growing-a-human (9/9/2026)

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

