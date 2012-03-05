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
    <div class="span2">
      <!--Sidebar content-->

      test

<script charset="utf-8" src="http://widgets.twimg.com/j/2/widget.js"></script>
<script>
new TWTR.Widget({
  version: 2,
  type: 'profile',
  rpp: 5,
  interval: 30000,
  width: 250,
  height: 400,
  theme: {
    shell: {
      background: '#333333',
      color: '#ffffff'
    },
    tweets: {
      background: '#000000',
      color: '#ffffff',
      links: '#4aed05'
    }
  },
  features: {
    scrollbar: true,
    loop: false,
    live: false,
    behavior: 'all'
  }
}).render().setUser('wadewegner').start();
</script>

    </div>
  </div>
</div>