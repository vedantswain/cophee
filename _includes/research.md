<!-- anchor hook for navbar -->
<span id="research"></span>

## Research

We leverage interdisciplinary approaches anchored around technological innovation to envision a new future of work and wellbeing. Our studies aim to contribute to the following intersecting areas. 

<div class="research-grid">
  {% for item in site.data.research %}
  <div class="research-item">
    <div class="research-content">
      <h3>{{ item.title }}</h3>
      <p>{{ item.description }}</p>
      {% if item.featured_papers %}
      <div class="featured-papers">
        <strong>Featured:</strong>
        {% for paper_id in item.featured_papers %}
          {% assign paper = site.data.bibliography | where: "id", paper_id | first %}
          {% if paper and paper.external_link %}
            <a href="{{ site.baseurl }}{{ paper.external_link }}" target="_blank">{{ paper.venue }}</a>{% unless forloop.last %}, {% endunless %}
          {% endif %}
        {% endfor %}
      </div>
      {% endif %}
    </div>
    <div class="research-image">
      <img src="{{ site.baseurl }}{{ item.image }}" alt="{{ item.alt }}" />
    </div>
  </div>
  {% endfor %}
</div>

For all published research, refer to Prof. Das Swain's [Google Scholar profile]({{ site.google_scholar }})


<!-- ### Selected Publications -->


<!-- {% assign grouped_papers = site.data.bibliography | group_by: "year" %}
{% for group in grouped_papers %}
<div class="papers">
  <h4>{{ group.name }}</h4>
  {% for paper in group.items %}
  <div class="paper-item">
    <span>{{ paper.title }}</span>
    {% if paper.award %}
      <i class="fa-solid fa-trophy" style="color: {% if paper.award == 'Best Paper' %}goldenrod{% else %}darkgoldenrod{% endif %};"></i>
    {% endif %}
    <br>
    {{ paper.author }} <br> 
    {{ paper.venue }} |
    <a href="{{ paper.external_link }}" target="_blank">Link</a>  
    {% if paper.internal_link %} | <a href="{{ paper.internal_link }}" target="_blank">PDF</a>{% endif %}
  </div>
  {% endfor %}
</div>
{% endfor %} -->
