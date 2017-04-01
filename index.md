---
layout: page
title: OpenTechSchool
tagline: "organizing tech workshops. Hands-on, awesome, and free."
---
{% include JB/setup %}

<div class="posts">
{% for post in site.posts %}

  <h2 class="post_title">
    <span><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></span>
  </h2>

  <span class="post_meta">

    {% if post.authors %}
      {% for author_id in post.authors %}
        {% assign author = site.authors[author_id] %}

        {% if author.link %}
          <a href="{{author.link}}">{{author.name}}</a>{% if forloop.last == false %}, {% endif %}
        {% else %}
          <a href="/authors.html#{{author_id}}">{{ author.name }}</a>{% if forloop.last == false %}, {% endif %}
        {% endif %}
        
      {% endfor %}

    {% else %}
      {% if post.author %}
        {% assign author_id = post.author %}
      {% else %}
          {% assign author_id = site.default_author %}
      {% endif %}    

      {% assign author = site.authors[author_id] %}

      {% if author.link %}
        <a href="{{author.link}}">{{author.name}}</a>
      {% else %}
        <a href="/authors.html#{{author_id}}">{{ author.name }} </a>
      {% endif %}
    {% endif %}
    &middot;    
    {{ post.date | date_to_long_string }}
  </span>

  <div class="post_content">
    {% if post.image %}
      <a class="header_image" href="{{ BASE_PATH }}{{ post.url }}">
        <img alt="{% if post.image_alt %}{{ post.image_alt|escape }} {% else %}{{ post.title|escape }}{% endif %}" src="{{ post.image }}" />
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

