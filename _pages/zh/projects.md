---
layout: page
title: 项目
permalink: /zh/projects/
lang: zh
lang_ref: projects
description: 一些软件、图形学和工程项目。
nav: false
nav_order: 5
horizontal: false
---

<div class="projects">
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
</div>
