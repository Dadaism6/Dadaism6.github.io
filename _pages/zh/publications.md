---
layout: page
permalink: /zh/publications/
title: 论文
lang: zh
lang_ref: publications
description: 论文、预印本与学术成果。
years: [2026,2025,2024,2023,2022]
nav: true
nav_order: 4
---

完整且持续更新的论文列表请见我的 <a href="https://scholar.google.com/citations?user={{ site.scholar_userid }}">Google Scholar profile</a>。

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
