---
layout: page
title: 教学
permalink: /zh/teaching/
lang: zh
lang_ref: teaching
description: 我教过的课
nav: true
nav_order: 6
horizontal: false
---

<h6>有个词叫“好为人师”。我爸经常说他自己当年应该去当个老师，有时候我也有同感，教课真的很好玩，也很有成就感。</h6>

<div class="projects">
  {%- assign sorted_teaching = site.teaching | sort: "importance" -%}
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_teaching -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_teaching -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
</div>
