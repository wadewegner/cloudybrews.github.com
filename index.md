---
layout: default
title: Cloudy Brews
tagline: Supporting tagline
---

<div class="container-fluid">
  <div class="row-fluid">
    <div class="span10">
		{% for post in site.posts limit:5 %}
		<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
		{{ post.content }}
		<em>Posted on {{ post.date | date_to_long_string }}.</em>
		{% endfor %}
    </div>
	<div class="span2 side-unit">
      <!--Sidebar content-->
      side
    </div>
  </div>
</div>



