<h2 id="services" style="margin: 2px 0px -15px;">Services</h2>

<div class="services">
<ol class="service-list">

{% for service in site.data.services.main %}

<li>
<div class="service-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if service.image %} 
    <img src="{{ service.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
    {% if service.category %} 
    <abbr class="badge">{{ service.category }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><strong>{{ service.title }}</strong></div>
      <div class="description">{{ service.description }}</div>
    <div class="links">
      {% if service.link %} 
      <a href="{{ service.link }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Learn More</a>
      {% endif %}
      {% if service.notes %} 
      <strong> <i style="color:#e74d3c">{{ service.notes }}</i></strong>
      {% endif %}
      {% if service.others %} 
      {{ service.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>
