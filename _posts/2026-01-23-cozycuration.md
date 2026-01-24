---
title: 'cozy curation'
date: 2026-01-23
#permalink: /posts
categories: Tiny_projects
laout: post
#comment: true
---

I love reading news articles and staying curious about whether my favorite writers have published something new, but I am super lazy. I do not like visiting their websites each time. Therefore, I prefer the traditional approach of using RSS. Actually, RSS feeds allow me to track new content on a website, instead of going to the site or subscribing to their emails. For me, it is super relaxing to get new updates without clutter. <br>
<br>
Initially, I searched for mobile RSS reader apps, but I could not find the best one for me. Those apps either had limited website support or required payment for full features. Hence, I forked [Static RSS reader generator](https://github.com/pesarkhobeee/lovelyRSS) made by [paraphobia](https://github.com/pesarkhobeee). I am happy with it. Currently, I am following ~30 sites, some of them update multiple times a day while other only few times a year. 
<br>
[Here is my curated RSS feeds](https://kabiraj404.github.io/free/ ) 
<br>
<br>
Likewise, I wanted to keep the list of sites that I have read on the interest. 
Bookmarking every page was not reasonable idea. I was inspired from [James' read list ](https://read.jamesst.one/). James reading list goes back to year 2022. I really loved James idea and inspired by it. I tried to fork and use it, but I could not replicate it. It might be due to my limited knowledge on programming. Hence, I created my own style. My approach is simple: first, I created a browser bookmarklet to grab website information using JavaScript. This bookmarklet logs the website's name and my feedback into a list in the github repository. The html based website grabs the information from this list to display my reading list. <br>
I am not good in in JavaScript and other language, I know bits and pieces of html, so I took help from LLM. This almost complete and updated list of articles I have read on the internet is not for judgment but just for memory. <br>
I might add some summary plots or other analysis chart, after I gather some data. <br>
[Here is my curated reading list](https://kabiraj404.github.io/ReadingCatalog/ )
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

