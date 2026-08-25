---
title: 'cozy curation'
date: 2026-07-22
#permalink: /posts
categories: Tiny_projects
laout: post
#comment: true
---

I love reading news articles and staying curious about whether my favorite writers have published something new, but I am super lazy. I do not like visiting their websites each time. Therefore, I prefer the traditional approach of using RSS. Actually, RSS feeds allow me to track new content on a website, instead of going to the site or subscribing to their emails. For me, it is super relaxing to get new updates without clutter. <br>
<br>
Initially, I searched for mobile RSS reader apps, but I could not find the best one for me. Those apps either had limited website support or required payment for full features. Hence, I forked [Static RSS reader generator](https://github.com/pesarkhobeee/lovelyRSS) made by [paraphobia](https://github.com/pesarkhobeee). I am happy with it. Currently, I am following ~30 sites, some of them update multiple times a day while other only few times a year. 
<br>
[Here is my curated RSS feeds](https://kabiraj404.github.io/rss/ ) 
<br>
Currently, it follows 32 sites, grouped together as data science, periodicals, photogrphy, periodical curated blogs and personal blogs. The slight update from the original rss fork is that it is more minimalist, and there is option to view all the list of the latest article, and a tab showing publiation from all the categories together. I believe it lets us follow our favorite topics and view direct headlines from specific sources.
<br>
I will try to maintain it. 
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

