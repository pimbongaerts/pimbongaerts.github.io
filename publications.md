---
layout: default
title: Publications
permalink: /publications/
---
## Selected publications

<ul>
{% assign sorted_pubs = site.data.publications.publications | sort: 'year' | reverse %}
{% assign previous_year = 0 %}
{% for publication in sorted_pubs %}
  {% if previous_year != publication.year %}
    <h2>{{ publication.year }}</h2>
  {% endif %}
  <li>
  	{{ publication.authors }}
  	({{ publication.year }})
  	<a href="{{ publication.pub_url  | escape}}">{{ publication.title }}</a>.
  	<strong>{{ publication.journal | escape }}</strong>
    {{ publication.volume | escape }} 
    {{ publication.pages | escape }}
    <br><br>
  </li>
  {% assign previous_year = publication.year %}
{% endfor %}
</ul>