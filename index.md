---
layout: page
title: The OpenTechSchool Blog
tagline: bringing free tech workshops to women and their friends
---
{% include JB/setup %}

<div class="posts">
{% for post in site.posts %}
  <h2 class="post_title">
    <span><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></span>
  </h2>

  <span class="post_meta">
    {% if post.author %}
      {{ post.author }}
    {% else %}
      {{ site.author.name }} 
    {% endif %}
    &middot;    
    {{ post.date | date_to_long_string }}
  </span>

  <div class="post_content">
    {% if post.teaser %}
      {{ post.teaser | markdownify }} 
      <a class="ots_action read_more" href="{{ BASE_PATH }}{{ post.url }}">Read&nbsp;more&nbsp;&#8594;</a>
    {% else %}
      {{ post.content }}
    {% endif %}
  </div>
{% endfor %}
</div>
