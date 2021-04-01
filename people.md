---
layout: default
title: People
permalink: /people/
---
<h2>Current lab members</h2>
<ul>
{% for person in site.data.people[] %}
  <li>
    <a href="{{ person.url }}">
      <img src="{{ person.image }}"><br>
      {{ person.name }}<br>
      <small>{{ person.title }}</small>
    </a>
  </li>
{% endfor %}
</ul>

<h2>Lab alumni</h2>
<ul>
{% for person in site.data.alumni %}
  <li>
    <a href="{{ person.url }}">
      <img src="{{ person.image }}"><br>
      {{ person.name }}<br>
      {{ person.title }}
    </a>
  </li>
{% endfor %}
</ul>