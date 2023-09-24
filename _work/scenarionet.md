---
layout: page
title: ScenarioNet
description: Open-source platform for large-scale traffic scenario modeling and simulation
img: assets/img/snet.jpg
importance: 1
category: research
---
From 2022.3 to present. UCLA Prof Bolei-Zhou's group.

- Latest news: The work has been accept by `NeuralIPS 2023 track on Datasets and Benchmarks`! Camera-ready paper will be released shortly.

<b>ScenarioNet</b> is an open-sourced platform for large-scale traffic scenario modeling and simulation.
<li>
    ScenarioNet defines a unified scenario description format containing HD maps and detailed object annotations.
</li>
<li>
    Scenarios recorded in this format can be replayed in the digital twins with multiple views, ranging from Bird-Eye-View layout to realistic 3D rendering.
</li>
<li>
    ScenarioNet provides tools to build and manage databases
    built from various data sources including real-world datasets like Waymo, nuScenes, Lyft L5, and nuPlan datasets and synthetic datasets like the procedural generated ones and safety-critical ones.
</li>
<li>
    We demonstrate several applications of ScenarioNet including large-scale scenario generation, AD testing, imitation learning, and reinforcement learning in both single-agent and multi-agent settings.
    The results imply scaling up the training data brings new research opportunities in machine learning and autonomous driving.
</li>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/snet.jpg" title="ScenarioNet Structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    ScenarioNet consists of the data layer, system layer, and application layer. Various datasets are unified into an internal scenario description. The system layer then provides a set of tools to operate on data efficiently, such as filtering, merging, sanity-check, splitting and so on. Once the database is ready, it can be loaded into MetaDrive for large-scale simulation and supports applications.
</div>