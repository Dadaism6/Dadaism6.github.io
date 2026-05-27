---
layout: about
title: About
permalink: /
lang: en
lang_ref: about
subtitle: ECE PhD @ UCLA | Research Intern @ Alibaba Accio | MS. CS 24' | BS. CS 22'
nav_order: 1
profile:
  align: right
  image: chenda_newpic.png
  image_circular: True # crops the image to make it circular
  address: >
    <p>Los Angeles, CA</p>
    <p>Email: chenda@ucla.edu</p>

news: true  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---
<!-- 🔍 **Actively Seeking Opportunities**:
- **2026 Summer Internship / 2026 Winter and Spring Part-time Internship** as a Research Scientist, Machine Learning Engineer, or Quant Researcher in the US.

If you believe there's a potential fit, please feel free to [email me](mailto:chenda@ucla.edu). I'm eager to explore new challenges and collaborations. -->

<h2 style="margin-top: 50px;">About me</h2>
<div class="abstract-block" markdown="1">
<div class="abstract-paragraph" markdown="1">
Hello there! I'm Chenda Duan, `a second-year Ph.D. student in Computer Engineering at UCLA`, where I am fortunate to be advised by Prof. [Vwani Roychowdhury](https://www.vwaniroychowdhury.com/). I am currently also an intern at `Alibaba Accio`, where I do Agentic Post-Training.
</div>

<div class="abstract-paragraph" markdown="1">
I earned both my B.S. and M.S. degrees in Computer Science from UCLA as well, conducting my master's research under the guidance of Prof. [Bolei Zhou](https://boleizhou.github.io/). During my bachelor's studies, I had the opportunity to work with Prof. [M. Khalid Jawed](https://structures.computer/) and Dr. [Roel Ophoff](https://bri.ucla.edu/people/roel-ophoff/). I am a 10-year UCLA Bruin!
</div>

<div class="research-blocks">
  <p class="research-label">Research directions</p>

  <div class="research-block" markdown="1">
  <h3>Agentic post-training</h3>
  At Alibaba Accio, I am the **core owner** of the training effort for `Accio’s next-generation agentic model`, focusing on agentic post-training, RL pipelines, interactive agent-environment infrastructure, and scalable training systems.
  </div>

  <div class="research-block" markdown="1">
  <h3>LLM/VLM memory and reasoning</h3>
  My current research lies in inference-time augmentation for `LLMs/VLMs` and `post-training` for LLMs. I am building next-generation RAG and structured memory systems with agentic design to enable better long-context understanding, multimodal reasoning, and agentic video understanding. More recently, I have been working on memory structures for agents, with the goal of helping LLMs/VLMs organize, retrieve, and reason over long-horizon context more effectively.
  </div>

  <div class="research-block" markdown="1">
  <h3>AI for Neuroscience</h3>
  A second line of my research focuses on `AI for Neuroscience`, where I develop machine learning systems for decoding human memory and cognition from neural activity. More broadly, I aim to bridge neuroscience and artificial intelligence in both directions: using AI to uncover the neural basis of memory and cognition, and drawing inspiration from the brain to design more adaptive architectures and learning algorithms.
  </div>
</div>

<div class="abstract-paragraph" markdown="1">
My previous research experience spans `autonomous driving`, `reinforcement learning`, `robotics`, and `biomedical AI`.
</div>
</div>


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

The field of computer science is vast and ever-evolving. Within this expansive domain, it is hard to constrain yourself into a specific area of interest. I am a firm believer in the power of interdisciplinary research and the importance of a broad skillset. I am passionate about the intersection of machine learning, medical science/neurosicence, computer vision, LLMs, and robotics.

**Research Interests**:
- LLM, VLM
- AI for Science
- Autonomous Systems and Robotics
- Reinforcement Learning


At UCLA, I've been fortunate to collaborate with three prominent research teams:

**Research Groups**:
- UCLA Prof Vwani Roychowdhury's Group
- UCLA Prof Bolei Zhou'S Group
- UCLA's Center for Neurobehavioral Genetics.
- UCLA Structures-Computer Interaction Lab.


For more information about me, connections, or just a friendly chat, all contact and social media details are available below.
