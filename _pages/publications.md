---
layout: page
permalink: /publications/
title: publications
order: 2
description: Che-Yi's publication.
years: [2022, 1956, 1950, 1935, 1905]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
