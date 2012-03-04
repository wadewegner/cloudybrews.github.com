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
    <p class="meta">{{ post.date | date: "%B %d, %Y" }}</p>
		{{ post.content }}
		<!--<em>Posted on {{ post.date | date_to_long_string }}.</em>-->
		{% endfor %}
    </div>
	<div class="span2">
      <!--Sidebar content-->
      Something will eventually go here. Not sure what.
    </div>
  </div>
</div>