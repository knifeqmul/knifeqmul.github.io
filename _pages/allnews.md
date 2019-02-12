---
title: "News"
layout: textlay
excerpt: "Knowledge Discovery from Health Use Data"
sitemap: false
permalink: /allnews
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
