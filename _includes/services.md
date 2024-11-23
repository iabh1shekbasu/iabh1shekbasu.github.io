{%- if site.data.services.teaching_assistant %}
Teaching Assistant Experience
<div class="services-container">
{% for position in site.data.services.teaching_assistant %}
  <div class="service-item">
    <h3>{{ position.course }}</h3>
    <p>{{ position.term }}</p>
    <p>Professor: {% if position.professor.link %}<a href="{{ position.professor.link }}">{{ position.professor.name }}</a>{% else %}{{ position.professor.name }}{% endif %}</p>
  </div>
{% endfor %}
</div>
{%- endif %}
{%- if site.data.services.conference_volunteering %}
Conference Volunteering
<div class="services-container">
{% for role in site.data.services.conference_volunteering %}
  <div class="service-item">
    <h3>{{ role.role }}</h3>
    <p><strong>{{ role.conference }}</strong></p>
    <p>Location: {{ role.location }}</p>
  </div>
{% endfor %}
</div>
{%- endif %}
