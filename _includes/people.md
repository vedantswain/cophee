<!-- anchor hook for navbar -->
<span id="people"></span>

### Students

Prof. Das Swain's fellowship at Northeastern allowed him to act as a Principal Investigator on projects and thus supervise and fund some extremely talented student researchers.  We are now looking to build an equally talented, capable, and responsible research group at NYU.

<ul>
  {% for student in site.data.people.students %}
    <li>
      <a href="{{ student.link }}">{{ student.name }}</a>
      &mdash; {{ student.role }}
    </li>
  {% endfor %}
</ul>

### Collaborators
<ul>
  {% for collaborator in site.data.people.collaborators %}
    <li>
      <a href="{{ collaborator.link }}">{{ collaborator.name }}</a> ({{ collaborator.affiliation }})
    </li>
  {% endfor %}
</ul>