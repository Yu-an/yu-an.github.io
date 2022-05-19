---
layout: page
permalink: /publications/
title: publications
years: [to appear,2022, 2021, 2020, 2017, 2016]
---
{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}