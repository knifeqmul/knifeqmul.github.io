﻿---
title: "KNIFE - Background"
layout: gridlay
excerpt: "KNIFE -- Background."
sitemap: false
permalink: /background/
---



## Staff 
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>  
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <i><li> {{ member.education1 }} </li></i>
  {% endif %}

  {% if member.number_educ == 2 %}
  <i><li> {{ member.education1 }} </li></i>
  <i><li> {{ member.education2 }} </li></i>
  {% endif %}

  {% if member.number_educ == 3 %}
  <i><li> {{ member.education1 }} </li></i>
  <i><li> {{ member.education2 }} </li></i>
  <i><li> {{ member.education3 }} </li></i>
  {% endif %}

  {% if member.number_educ == 4 %}
  <i><li> {{ member.education1 }} </li></i>
  <i><li> {{ member.education2 }} </li></i>
  <i><li> {{ member.education3 }} </li></i>
  <i><li> {{ member.education4 }} </li></i>
  {% endif %}

  {% if member.number_educ == 5 %}
  <i><li> {{ member.education1 }} </li></i>
  <i><li> {{ member.education2 }} </li></i>
  <i><li> {{ member.education3 }} </li></i>
  <i><li> {{ member.education4 }} </li></i>
  <i><li> {{ member.education5 }} </li></i>
  {% endif %}
  </ul>
  
{{ member.info }}
</div>
    
 
{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Researcher

