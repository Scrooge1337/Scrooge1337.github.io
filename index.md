---
layout: default
title: Der wundersame Blog des Sebastian Reimers
---
<div class="homecontent">
  {% for post in site.posts %}
  <a class="kartenlink" href="{{ post.url }}">
      <div class="karte" data-tilt>
        <h4 class="indextitle postlink">{{ post.title }}</h4>
        <desc>{{ post.date | date_to_string }}</desc>
        <div class="postpreview" >
          <img class="postthumbnail"  src="{{ post.image }}">
          <div class="postdescription">{{ post.description }} </div>
        </div>
      </div>
    </a>
{% endfor %}
</div>
