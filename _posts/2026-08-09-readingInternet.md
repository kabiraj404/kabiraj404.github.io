---
title: 'Read list '
date: 2026-08-09
#permalink: /posts
categories: Tiny_projects
laout: post
#comment: true
---


I loved to keep track of sites, blogs, and other items that I have read on the interest. Bookmarking every page on the browser was not reasonable idea.<br>

I was inspired from [James’ read list](https://read.jamesst.one/) and [abi abi's reading list](https://read.jamesst.one/). Abi's reading list goes back to year 2021 and James back to 2022. I really loved James’s idea and inspired by it. <br> 
I thought to try it myself and keep track of anyting that I read on the internet. <br> 
I tried to fork and use their repository, but I could not replicate it. It might be due to my limited knowledge of programming. Hence, I created my own style. My approach is simple: first, I created a browser bookmarklet to grab website information using JavaScript. This bookmarklet logs the website’s name and my feedback into a list in the GitHub repository. The html-based website grabs the information from this list to display my reading list. 
I am not good at JavaScript and other languages, I know bits and pieces of html, so I got help from LLM for JavaScript for bookmarking. <br>
This almost complete and updated list of articles I have read on the internet is not for judgment but just for memory. <br>
I might add some summary plots or other analysis charts, after I gather some data. <br>
<br>
[Here is my curated reading list](https://kabiraj404.github.io/ReadingList/) 
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

