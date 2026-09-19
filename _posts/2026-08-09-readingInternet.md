---
title: 'My reading list '
date: 2026-08-09
#permalink: /posts
categories: Tiny_projects
laout: post
#comment: true
---


I loved to keep track of sites, blogs, and other items that I have read on the interest. Bookmarking every page on the browser was not reasonable idea.<br>

I was inspired from [James’ read list](https://read.jamesst.one/) and [abi abi's reading list](https://read.jamesst.one/). Abi's reading list goes back to year 2021 and James back to 2022. I really loved James’s idea and inspired by it. I thought to try it myself and keep track of anyting that I read on the internet. I tried to fork and use their repository, but I could not replicate it. It might be due to my limited knowledge of programming. <br>
Hence, I created my own style. My approach is simple, scrap the website name, tile of the article and link to the article, add my persoanal thoughts and save it to the github as a list. I created a browser bookmarklet to grab website information using JavaScript. I am not good at JavaScript, I know bits and pieces of html, so I got help from LLM for JavaScript for bookmarking strategy so that it can be uploaded to the github repository. This bookmarklet captures the website’s name, date of entry and while doing this, I add my personal thoughts in a few words and it will collect all teh informaiton as a list in the GitHub repository. The html-based website grabs the information from this list to display my reading list. 
 <br>
This almost complete and updated list of articles I have read on the internet is not for judgment but just for memory. <br>

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

