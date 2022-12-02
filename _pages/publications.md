---
layout: page
permalink: /publications/
title: Publications
description:
years: [2022,2021,2020,2019,2018,2017,2016,2014]
nav: true
nav_order: 1
dropdown: true
children:
    - title: Patents
      permalink: /patents/
    - title: divider
    - title: Books
      permalink: /bpublications/
    - title: divider
    - title: Journals
      permalink: /publications/
    - title: divider
    - title: Conferences
      permalink: /cpublications/

---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f jpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>
