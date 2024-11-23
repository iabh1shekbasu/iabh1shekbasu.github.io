---
layout: page
title: Services
---

<h2 id="services" style="margin: 2px 0px -15px;">Services</h2>

<div class="services">
  <ol class="service-list">
    {% for category, items in site.data.services %}
      <li>
        <h3>{{ category | replace: '_', ' ' | capitalize }}</h3>
        <ul>
          {% for item in items %}
            <li>
              {% if item.course %}
                <strong>{{ item.course }}</strong> - {{ item.term }}
                <br>Professor: <a href="{{ item.professor.link }}">{{ item.professor.name }}</a>
              {% endif %}
              {% if item.role %}
                <strong>{{ item.role }}</strong>
                <br>Conference: {{ item.conference }}
                <br>Location: {{ item.location }}
              {% endif %}
            </li>
          {% endfor %}
        </ul>
      </li>
    {% endfor %}
  </ol>
</div>
