---
layout: page
permalink: /bpublications/
title: Books
description:
years: [2021]
nav: false
nav_order: 7
---
<!-- _pages/bpublications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f pbooks -q @*[year={{y}}]* %}
{% endfor %}

</div>
