---
layout: page
title: OpenTechSchool Authors
---
{% include JB/setup %}

## The Authors

<div class="team_list">
{% for author_data in site.authors %}
	{% assign author_id = author_data[0] %}
	{% assign author = author_data[1] %}
<div class="{% cycle 'left', 'right' %}">
	{% if author.image %}
		<img src="{{author.image}}" >
	{% endif %}

	<h3 id="{{author_id}}">{{author.name}}</h3>
	<p>{{author.about}}</p>
	<p><a href="mailto: {{author.email}}">{{author.email}}</a></p>
</div>
{% endfor %}
</div>