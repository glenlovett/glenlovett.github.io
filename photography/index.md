---
layout: default
title: Photography
---

## Galleries

{% for gallery in site.data.galleries %}
  <br />
  [> {{ gallery.description }} *({{gallery.images.size}} Images)*
    <img src="{{ gallery.imagefolder }}/{{gallery.images.first.thumb}}" class="desaturate">
  ]({{ gallery.id }})
{% endfor %}