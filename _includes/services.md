# Services

### Teaching Assistant Experience

{% raw %}
{%- if site.data.services.services.teaching_assistant %}
<div class="services-container">
{%- for position in site.data.services.services.teaching_assistant %}
  <div class="service-item">
    <h3>{{ position.course }}</h3>
    <p>{{ position.term }}</p>
    <p>Professor: {% if position.professor.link %}<a href="{{ position.professor.link }}">{{ position.professor.name }}</a>{% else %}{{ position.professor.name }}{% endif %}</p>
  </div>
{%- endfor %}
</div>
{%- endif %}

### Conference Volunteering

{%- if site.data.services.services.conference_volunteering %}
<div class="services-container">
{%- for role in site.data.services.services.conference_volunteering %}
  <div class="service-item">
    <h3>{{ role.role }}</h3>
    <p><strong>{{ role.conference }}</strong></p>
    <p>Location: {{ role.location }}</p>
  </div>
{%- endfor %}
</div>
{%- endif %}
{% endraw %}
