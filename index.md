---
layout: default
title: Der wundersame Blog des Sebastian Reimers
---
{% for post in site.posts %}
  <h4 class="indextitle"><a href="{{ post.url }}" class="postlink">{{ post.title }}</a></h4>
  <desc>{{ post.date | date_to_string }}</desc>
  <div class="postdescription">{{ post.description }} </div>
{% endfor %}