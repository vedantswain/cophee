
<p style="text-align: left;">
{% for item in site.data.activity %}
<small>
  <i class="{{ item.icon }}"></i>
  <a href="{{ item.link }}">{{ item.description }}</a>
</small></br>
{% endfor %}
</p>
