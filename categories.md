---
layout: page
title: categories
permalink: /categories/
---
<a href="/blog-posts">all blog posts< </a>  
<br>
{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
  	{% for post in category[1] %}
  	  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %} 
  </ul>
{% endfor %}

