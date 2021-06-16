---
layout: default
title: Publications
permalink: /publications/
---
## Selected publications

<ul>
{% assign sorted_pubs = site.data.publications.publications | sort: 'year' | reverse %}
{% for publication in sorted_pubs %}
  <li>
  	{{ publication.authors }}
  	({{ publication.year }})
  	{{ publication.title }}.
  	<strong>{{ publication.journal | escape }}</strong>
    {{ publication.volume | escape }}:
    {{ publication.pages | escape }}
    (<a href="{{ publication.pub_url  | escape}}">link</a> / citations:  {{ publication.citations | escape }})
  </li>
{% endfor %}
</ul>