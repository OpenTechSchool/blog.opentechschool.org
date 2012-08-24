---
layout: page
title: OpenTechSchool Blog
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
    {% if post.image %}
      <a class="header_image" href="{{ BASE_PATH }}{{ post.url }}">
        <img alt="{{ post.title }}" src="{{ post.image }}" />
      </a>
    {% endif %}
    {% if post.teaser %}
      {{ post.teaser | markdownify }} 
      <a class="ots_action read_more" href="{{ BASE_PATH }}{{ post.url }}">Read&nbsp;more&nbsp;&#8594;</a>
    {% else %}
      {{ post.content }}
    {% endif %}
    <a class="comments_action" href="{{ BASE_PATH }}{{ post.url }}#disqus_thread">Leave a comment!</a>
  </div>
{% endfor %}
</div>

<script type="text/javascript">
  /* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
  var disqus_shortname = '{{ site.JB.comments.disqus.short_name }}'; 
  
  /* * * DON'T EDIT BELOW THIS LINE * * */
  (function () {
    var s = document.createElement('script'); s.async = true;
    s.type = 'text/javascript';
    s.src = 'http://' + disqus_shortname + '.disqus.com/count.js';
    (document.getElementsByTagName('HEAD')[0] || document.getElementsByTagName('BODY')[0]).appendChild(s);
  }());
</script>

