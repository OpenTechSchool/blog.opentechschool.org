---
layout: page
title: blog.OpenTechSchool.org!
tagline: bringing free tech workshops to women and their friends
---
{% include JB/setup %}

<div class="posts">
{% for post in site.posts %}
<div class="multi-post-wrap">
  <h2 class="post-title">
    <span class="post-date">{{ post.date | date_to_string }}</span> &raquo;
    <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
  </h2>
  <div class="post-content">
    {{post.content}}
  </div>
</div>
{% endfor %}
</div>
