---
title: 'Cozy curation'
date: 2026-01-23
#permalink: /posts
categories: projects
laout: post
#comment: true
---

I love reading news articles and staying curious about whether my favorite writers have published something new, but I am super lazy. I do not like visiting their websites each time. Therefore, I still prefer the traditional approach of using RSS. <br>
<br>
RSS feeds allow us to track changes or new content on a website. Instead of going to the site or subscribing to emails, a website's RSS feed allows us to see updates in one place. It super relaxing to get all new updates from our favorite website automatically in one location without clutter. <br>
<br>
Initially, I searched for mobile RSS reader apps, but I could not find the best one for me. Those apps either had limited website support or required payment for full features. Hence, I forked [Static RSS reader generator](https://github.com/pesarkhobeee/lovelyRSS) made by [paraphobia](https://github.com/pesarkhobeee). So far, I am having really good experince. Currently, I am following ~30 sites, some of them update multiple times a day while other only few times a year. 
<br>
[Here is my curated RSS feeds](https://kabiraj404.github.io/free/ ) 
<br>
<br>
Likewise, I wanted to keep the list of sites that I have read on the interest. 
Bookmarking every page was not reasonable idea. Hence, I created almost complete and updated list of articles I have read on the internet. It is not for judgment but just for memory. <br>
<br>
[Here is my curated reading list]( https://kabiraj404.github.io/ReadingCatalog/ )
<br>
I was inspired from [James' read list ] (https://read.jamesst.one/). James list goes back to 2022. I really love and respect James idea.  I tried to fork and use it, but I could not replicate it. It might be due to my limited knowledge on programming, so I created my own style. My approach is simple: first, I created a browser bookmarklet to grab website information using JavaScript. As I use this bookmarklet, it logs the website's name and my feedback into a list. This list is displayed on the website by using html. Honestly, LLM helped me convert this idea into reality because I am not good in JavaScript. <br>
I might add some summary plot or other analysis after I gather some data on what I am reading.  

Happy reading. 
<br>
<br>
This blog appears in the category: 
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

