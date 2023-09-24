---
layout: page
title: Proxy Value Propagation
description: A safe and super-efficient human-in-the-loop reinforcement learning method!
img: assets/img/realrendering.png
importance: 1
category: research
---
From 2022.3 to present. UCLA Prof Bolei-Zhou's group.

- Latest news: The work has been accept by `NeuralIPS 2023` as a `Spotlight Paper`! Camera-ready paper will be released shortly.

I’m excited to share my latest research paper on enhancing AI learning through active human involvement. This approach introduces a novel method, "Proxy Value Propagation," for policy optimization, ensuring safety and AI alignment in training. The core idea is to design a proxy value function to represent human intents, assigning high values to human demonstrations and low values to intervened agent actions. This method successfully emulates human behaviors across various tasks, including the challenging driving task in Grand Theft Auto V. Demo video and code will be made public soon. Looking forward to further exploring this impactful field!

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pvp_main_exp.jpg" title="PVP exp demo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The method can be applied to various tasks, including the challenging driving task in Grand Theft Auto V. It is super efficient.
</div>