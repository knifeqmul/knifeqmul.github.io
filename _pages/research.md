---
title: "KNIFE - Research Updates"
layout: gridlay
excerpt: "KNIFE -- Research Updates."
sitemap: false
permalink: /research/
---



# Research Updates

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}



## Issues
1. Data is in CCG, while GPs are located in clinics.
2. Data is semi-structured without clear description.



## To do
1. Ontology.
2. EHR applications.
3. Causal hypothesis testing.

