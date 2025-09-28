---
layout: page
permalink: /publications/
title: Publications
description: Reviewer for T-ITS, NIPS 2025, AAAI 2026, ICLR 2026
years: [2025,2024,2023, 2022]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
