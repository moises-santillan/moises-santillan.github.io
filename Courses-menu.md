---
layout: page
title: Courses
permalink: /courses-menu/
nav-include: true
nav-order: 3
---

## Courses

Over time, I have taught the following courses. In the corresponding links you can find more information.

<ul class="course-list">
{% assign courses_coleccion = site.courses | sort: "course_id" %}
{% for course in courses_coleccion %}
  <li>
    <a href="{{ course.url | relative_url }}">
      <strong>{{ course.title }}</strong>
      </a>
  </li>
{% endfor %}
</ul>
