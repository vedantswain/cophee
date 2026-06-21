---
title: Alumni
layout: article
---

# Alumni

Prof. Das Swain has mentored students in the capactity of a PI or Co-PI in NYU and during his fellowship at Northeastern.

<ul>
  {% for student in site.data.people.students %}
  {% if student.tenure == "past" %}
    <li>
      <a href="{{ student.link }}">{{ student.name }}</a>
      &mdash; {{ student.role }}
    </li>
  {% endif %}
  {% endfor %}
</ul>
