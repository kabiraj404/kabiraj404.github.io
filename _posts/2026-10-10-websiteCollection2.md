---
title: 'Useless links 2026-10'
date: 2026-10-01
#permalink: /posts
categories: Collection
laout: post
#comment: true
---

Here is a list of websites I found interesting this month.


**Book collections** (Accessed Sep 10, 2026)
* [Classic Archive](https://classics.mit.edu/index.html)
* [Wisdom Library](https://www.wisdomlib.org/hinduism/book/shiva-purana-english)

**RSS** (Accessed Sep 10, 2026)
* [State of art on RSS](https://github.com/AboutRSS/ALL-about-RSS?tab=readme-ov-file#apps)
* [Email newsletter to RSS](https://kill-the-newsletter.com/)
* [RSS from webpage](https://rss-bridge.org/bridge01/)


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

