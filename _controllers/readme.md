---
permalink: /controllers/index.html
layout: default
title: 控制器
---

<h2>控制器</h2>

<ul>
{% for item in site.controllers limit:16 %}
 {% if item.title != "Readme" and item.title != "控制器" %}
 <li><a href="{{ item.url | downcase}}">
 <p>{{ item.title }}</p>
 <p>{{ item.description }}</p>
 </a></li>
 {% endif %}
{% endfor %}
</ul>
