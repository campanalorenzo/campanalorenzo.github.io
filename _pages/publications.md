---
layout: page
permalink: /publications/
title: publications
description: articles, conference papars, thesis in reversed chronological order. 
years: [2022, 2019, 2017]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}




