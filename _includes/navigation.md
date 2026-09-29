<nav>
  <p class="site-title"><a href="{{ "/" | absolute_url }}">{{ site.name }}</a></p>
  <button type="button" class="burger" aria-label="Menu" aria-expanded="false" aria-controls="nav-links">
    <i class="fa-solid fa-bars" style="font-size:1.1rem" aria-hidden="true"></i>
  </button>
  <div class="nav-links" id="nav-links">
    {% for item in site.data.navigation %}
      <a href="{{ item.link }}">{{ item.name }}</a>
    {% endfor %}
  </div>
</nav>