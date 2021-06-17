---
layout: default
title: Outreach
permalink: /outreach/
---

<h2>Videos & broadcasts</h2>
<ul class="videos">
{% for video in site.data.videos %}
  <li>
    {{ video.outlet }} - {{ video.title }}
    <iframe width="320" height="180" src="https://www.youtube.com/embed/{{ video.youtube_id }}" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe><br><br>
  </li>
{% endfor %}
</ul>