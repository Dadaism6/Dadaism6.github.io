---
layout: about
title: About
permalink: /
subtitle: UCLA MS. Computer Science 24' | BS. Computer Science 22'
nav_order: 1
profile:
  align: right
  image: chenda_pic.jpg
  image_circular: True # crops the image to make it circular
  address: >
    <p>Los Angeles, CA, 90024</p>
    <p>Phone: 310-254-5864</p>
    <p>Email: chenda@ucla.edu</p>

news: true  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---
<h2 style="margin-top: 50px;">About me</h2>
Hello! I'm Chenda Duan, `a second-year MS student in Computer Science at UCLA`, previous interning as a `Machine Learning Research Engineer` at Kuaishou Technology this summer. I recently graduated with a B.S. in Computer Science from UCLA, proudly with a perfect `4.0 GPA`.

🔍 **Actively Seeking Opportunities**:
- **PhD opportunities** focusing on Multi-modal Learning, RL, AI for Medicine/Bio, and general AIGC.
- **Full-time roles** as a Machine Learning Engineer, Software Engineer, or Quant Researcher in the US.

If you believe there's a potential fit, please [contact me](mailto:chenda@ucla.edu). I'm eager to explore new challenges and collaborations.

<div class="news">
  <h2 style="margin-top: 50px;">News</h2>
  {% if site.news != blank -%} 
  {%- assign news_size = site.news | size -%}
  <div class="table-responsive" {% if site.news_scrollable and news_size > 3 %}style="max-height: 10vw"{% endif %}>
    <table class="table table-sm table-borderless">
    {%- assign news = site.news | reverse -%}
    {% if site.news_limit %}
    {% assign news_limit = site.news_limit %}
    {% else %}
    {% assign news_limit = news_size %}
    {% endif %}
    {% for item in news limit: news_limit %} 
      <tr>
        <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
        <td>
          {% if item.inline -%} 
            {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
          {%- else -%} 
            <a class="news-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
          {%- endif %} 
        </td>
      </tr>
    {%- endfor %} 
    </table>
  </div>
{%- else -%} 
  <p>No news so far...</p>
{%- endif %} 
</div>

<h2 style="margin-top: 50px;">About my academics.</h2>

The field of computer science is vast and ever-evolving. Within this expansive domain, it is hard to constrain yourself into a specific area of interest. I am a firm believer in the power of interdisciplinary research and the importance of a broad skillset. I am passionate about the intersection of machine learning, computer vision, and robotics. I am also very interested in the application of machine learning in the field of Biology, Medicine, and Economics.

**Research Interests**:
- Reinforcement Learning
- Multi-modal Learning (Vision-language)
- AI for Medicine, Computational Bio
- Robotics


At UCLA, I've been privileged to collaborate with three prominent research teams:

**Research Groups**:
- UCLA Prof Bolei Zhou'S Group
- UCLA's Center for Neurobehavioral Genetics.
- UCLA Structures-Computer Interaction Lab.


For more information about me, connections, or just a friendly chat, all contact and social media details are available below.





