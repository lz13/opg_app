---
layout: single
title: Gallery
permalink: /gallery/
---

{% for image in site.static_files %}
  {% if image.path contains '/assets/img/gallery/' %}
    <img src="{{ site.baseurl }}{{ image.path }}" alt="{{ image.name }}" />
  {% endif %}
{% endfor %}