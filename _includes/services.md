# Academic Services

## Conference Reviewing

- 

## Teaching Assistant

{%- for position in site.data.services.services.teaching_assistant %}
- {{ position.course }} course - {{ position.term }} with 
  {%- for prof in position.professor -%}
    {%- if forloop.last and forloop.first -%}
      [{{ prof.name }}]({{ prof.link }})
    {%- elsif forloop.last -%}
      and [{{ prof.name }}]({{ prof.link }})
    {%- else -%}
      [{{ prof.name }}]({{ prof.link }}), 
    {%- endif -%}
  {%- endfor %}
{%- endfor %}

## Conference Volunteering

{%- for role in site.data.services.services.conference_volunteering %}
- {{ role.role }} - {{ role.conference }}, {{ role.location }}
{%- endfor %}
