---
layout: page
title: blorg-posts
permalink: /blorg-posts/
---
<a href="/">main menu< </a>  
<a href="/categories">post categories< </a>  
<br>
<h3>Posts</h3>  
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} >> {{ post.date }} </a>
    </li>
  {% endfor %}
</ul>