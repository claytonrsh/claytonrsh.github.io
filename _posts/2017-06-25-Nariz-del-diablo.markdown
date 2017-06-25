---
layout:     post
title:      "La Nariz del Diablo"
subtitle:   "The train to a view and back again."
date:       2017-06-25 09:55:00
author:     "Clayton"
header-img: "img/post11/IMG_1007.JPG"
---
{% assign post_data = site.data.post11 %}

<i>Another post on blogger about Ecuador. This was not at all about views, it was all about the train.<i/>

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
