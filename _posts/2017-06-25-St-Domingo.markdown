---
layout:     post
title:      "BU goes to St. Domingo... well close to it"
subtitle:   "Nearly nine years later..."
date:       2017-06-25 09:10:00
author:     "Clayton"
header-img: "img/post9/IMG_0951.jpg"
---
{% assign post_data = site.data.post9 %}

<i>Another post on blogger when I studied abroad in Ecuador...<i/>

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
