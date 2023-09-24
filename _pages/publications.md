---
layout: page
permalink: /publications/
title: Publications
description: Publications serve as vessels of knowledge, displaying the fruits of extensive labor, exploration, and discovery. Yet, beneath the polished surface of each paper, there lies a hidden ocean of unrevealed endeavors, a labyrinth of thoughts, trials, and tribulations that remain obscured in the shadows of the finalized work.
                    --- Chenda
years: [2023, 2022]
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
