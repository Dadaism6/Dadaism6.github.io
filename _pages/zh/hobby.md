---
layout: page
title: 爱好
permalink: /zh/hobby/
lang: zh
lang_ref: hobby
description: 实验室之外，我也会反复回到的一些事情。
nav: true
nav_order: 7
horizontal: false
---

<div class="projects">
  {%- assign sorted_hobby = site.hobby | sort: "importance" -%}
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_hobby -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_hobby -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
</div>
