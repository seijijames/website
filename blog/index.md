---
layout: default
title: blog
permalink: /blog/
---
 <p>blog</p>
 <article class="postpreview">
 {% for post in site.posts %}
    <h3>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
    <p class="post-date">
     <p>
      {{ post.date | date: "%B %-d, %Y" }}
    </p>
    <p>{{ post.summary }}</p>
    <p>
      <a href="{{ post.url | relative_url }}">read more →</a>
    </p>
  {% endfor %}
 </article>
 
