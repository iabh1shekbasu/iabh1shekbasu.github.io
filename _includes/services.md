# Academic Services

## Conference Reviewing

- 

## Teaching Assistant

{%- for position in site.data.services.services.teaching_assistant %}
- {{ position.course }} course - {{ position.term }} with [{{ position.professor.name }}]({{ position.professor.link }})
{%- endfor %}

## Conference Volunteering

{%- for role in site.data.services.services.conference_volunteering %}
- {{ role.role }} - {{ role.conference }}, {{ role.location }}
{%- endfor %}
