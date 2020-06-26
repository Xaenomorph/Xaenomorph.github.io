---
title: Blog
layout: blog
---


{% for post in site.posts %}
<br>

<img src="{{ post.img | prepend: site.baseurl }}" width="400" length="150">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date_to_string }}<p>
   {{ post.excerpt }}
  
  
<br>
  {% endfor %}
