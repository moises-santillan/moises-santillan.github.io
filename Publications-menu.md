---
layout: page
title: Publications
permalink: /publications-menu/
nav-include: true
nav-order: 2
---

## Publication Lists

Complete lists of published papers, books, book chapters and essays.

<ul class="publication-list">
{% assign sorted_publications = site.publications | sort: "type_id" %}
{% for publication-type in sorted_publications %}
  <li>
    <a href="{{ publication-type.url | relative_url }}"><strong>{{ publication-type.title }}</strong></a>
  </li>
{% endfor %}
</ul>