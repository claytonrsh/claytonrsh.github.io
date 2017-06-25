---
layout:     post
title:      "Six years later"
subtitle:   "Second attempt to put things on the web..."
date:       2017-06-25 09:40:00
author:     "Clayton"
header-img: "img/post10/IMG_5503.2015-01-05_185753.jpg"
---
{% assign post_data = site.data.post10 %}

<i>Another post on blogger, but this time after my mom visited me in Costa Rica.<i/>

<div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1">
{% for entry in post_data %}
  {% if entry.entry > 0 %}
    {% if entry.picture != "" %}
      <image src="{{ site.baseurl }}/img/{{ entry.picture }}">
      <figcaption>{{entry.caption}}</figcaption>
    {% endif %}
    {% if entry.picture == "" %}
      <p>{{ entry.caption }}</p>
    {% endif %}
    <br>
  {% endif %}
{% endfor %}
