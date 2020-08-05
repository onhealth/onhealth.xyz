---
layout: page
title: blog
---

# Blog Posts  
  
---------------------  
  
<div class="posts">
  {% for post in site.posts %}
    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
    <h3>{{ post.excerpt }}</h3>
    <h6>Posted by <a href="{{ post.url }}">{% if page.author %}{{ page.author }}{% else %}{{ site.author }}{% endif %}</a> on {{ post.date | date: '%B %d, %Y' }}</h6>
   <br>
   <hr>
  {% endfor %}
</div>
