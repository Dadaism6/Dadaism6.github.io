---
layout: page
permalink: /publications/
title: Publications
lang: en
lang_ref: publications
description: Reviewer for T-ITS, NIPS, AAAI, ICLR, CAIS
years: [2026,2025,2024,2023,2022]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->

For a complete and regularly updated publication list, please see my <a href="https://scholar.google.com/citations?user={{ site.scholar_userid }}">Google Scholar profile</a>.

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
