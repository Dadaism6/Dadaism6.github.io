---
layout: page
title: 研究经历
permalink: /zh/work/
lang: zh
lang_ref: work
description: 我做过的一些研究系统、论文和实验室项目。
nav: false
nav_order: 3
horizontal: false
---

<div class="projects">
  {%- assign sorted_work = site.work | sort: "importance" -%}
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_work -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_work -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
</div>
