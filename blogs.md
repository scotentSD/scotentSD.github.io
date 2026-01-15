---
layout: page
title: Blog
permalink: /blog-post-list/
---
<br>
<ul>
  {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}" class="blog-post-title">{{ post.title }}</a>
        <div class="date">	
            Written on {{ post.date | date_to_string }} {% if post.author %} by {{post.author}} {% endif %}          	
       </div>	
      {{ post.excerpt }}
      </li>
  {% endfor %}
  </ul>

<br><br>
<div>Last updated: {{site.time | date_to_string}}</div>


