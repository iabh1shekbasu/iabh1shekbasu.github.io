<h2 id="services" style="margin: 2px 0px -15px;">Services</h2>

<div class="services">
<ol class="service-list">
{% for category, items in site.data.services %}
  <li>
    <h3>{{ category | replace: '_', ' ' | capitalize }}</h3>
    <ul>
    {% for item in items %}
      <li>
        <strong>{{ item.course or item.role }}</strong>
        {% if item.term %} - {{ item.term }}{% endif %}
        {% if item.professor %}
          <br>Professor: <a href="{{ item.professor.link }}">{{ item.professor.name }}</a>
        {% endif %}
        {% if item.conference %}
          <br>Conference: {{ item.conference }}
        {% endif %}
        {% if item.location %}
          <br>Location: {{ item.location }}
        {% endif %}
      </li>
    {% endfor %}
    </ul>
  </li>
{% endfor %}
</ol>
</div>
