# Services

## Teaching Assistant Experience

{%- for position in site.data.services.services.teaching_assistant %}
<div class="service-item">
  <h3>{{ position.course }}</h3>
  <p>{{ position.term }}</p>
  <p>Professor: <a href="{{ position.professor.link }}">{{ position.professor.name }}</a></p>
</div>
{%- endfor %}

## Conference Volunteering

{%- for role in site.data.services.services.conference_volunteering %}
<div class="service-item">
  <h3>{{ role.role }}</h3>
  <p><strong>{{ role.conference }}</strong></p>
  <p>Location: {{ role.location }}</p>
</div>
{%- endfor %}
