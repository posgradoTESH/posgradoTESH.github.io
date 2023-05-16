---
layout: page
permalink: /publications/
title: Publicaciones
description: Publicaciones realizadas por los Docentes del Programa de Maestría en Ciencias de la Ingeniería
years: [2023, 2022, 2021, 2020]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
