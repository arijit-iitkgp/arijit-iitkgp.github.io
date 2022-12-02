---
layout: page
permalink: /cpublications/
title: Conferences
description:
years: [2022,2021,2020,2019,2018,2015,2014,2013]
nav: false
nav_order: 7
---
<!-- _pages/bpublications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f cpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>
