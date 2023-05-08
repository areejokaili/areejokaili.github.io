---
layout: page
permalink: /publications/
title: Publications
description: Full list of publications at <a style='color:#B509AC' href='https://scholar.google.com/citations?user=QI2gCEsAAAAJ&hl=en'>Google scholar</a> 
years: [ 2019, 2020]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
<p><b>{{y}}</b></p>
 <!--  <h2 class="year">{{y}}</h2> -->
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
