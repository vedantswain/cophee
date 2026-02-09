<!-- anchor hook for navbar -->
<span id="people"></span>

## People

<!-- ### Faculty -->
<div class="people">
{% for faculty in site.data.people.faculty %}
<div class="people core">
  {% if faculty.image %}
   <img src="{{ faculty.image }}" alt="{{ faculty.name }}" class="faculty-image" />
  {% endif %}
  <p><a href="{{ faculty.link }}">{{ faculty.name }}</a></p>
  <p>{{ faculty.role }}</p> 
  <p>{{ faculty.affiliation }}</p>
</div>
{% endfor %}

<!-- ### Current Students -->
{% for student in site.data.people.students %}
  {% if student.tenure == "current" %}
  <div class="people core">
    {% if student.image %}
     <img src="{{ student.image }}" alt="{{ student.name }}" class="faculty-image" />
    {% endif %}
    <p><a href="{{ student.link }}">{{ student.name }}</a></p>
    <p>{{ student.role }}</p>
    <p>{{ student.affiliation }}</p>
    
  </div>
  {% endif %}
{% endfor %}

</div>

### Former Students

Prof. Das Swain has mentored students at various capacities from the start of his PhD. Listed below are students he has advised as a PI or co-PI. 

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

### Collaborators

We have a growing list of experts across industry and academia who are collaborate with us on different projects:

<ul>
  {% for collaborator in site.data.people.collaborators %}
    <li>
      <a href="{{ collaborator.link }}">{{ collaborator.name }}</a> ({{ collaborator.affiliation }})
    </li>
  {% endfor %}
</ul>
