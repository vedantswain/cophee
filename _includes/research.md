<!-- anchor hook for navbar -->
<span id="publications"></span>

## Research

We leverage interdisciplinary approaches anchored around technological innovation to envision a new future of work and wellbeing.

**Human-Centered ML:**
Existing approaches to understand workers with data, rarely consider worker perspectives. We engage with data-subjects, like workers, to derive new designs for estimating behavioral health and guide these models to align ethically and practically with their social context.

**Social-Ecological Informatics:**
Traditional ways of describing workers does not reflect how social relationships affect their behaviors. We contextualize situations with multimodal data and demonstrate computational models that highlight overlooked factors associated with healthier organizational practices.

**Digital Wellbeing Interventions:**
Performance and wellness are often viewed as mutually exclusive, but we show that we can augment work routines to ensure sustainable effectiveness. We develop AI and computational applications for task-level and day-level activities to mitigate negative challenges to mental health.

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
