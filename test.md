---
layout: page
title: journal
permalink: /categories/journal
---
{% for cat in site.categories %}
{% if cat[0] == 'journal' %}
  <h3>{{ cat[0] }}</h3>
{% for post in cat[1] %}
  <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
{% endif %}
{% endfor %}