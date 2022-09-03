---
layout: page
title: Googolplex
description: Online text generation server
img: assets/img/googolplex.png
importance: 1
category: project
---
This is my final project for UCLA CS130: Software Engineering. Our group is called "googolplex", which is simply 10 to the power of many, many...

Source code at: <a href="https://github.com/Dadaism6/UCLA-CS130-Googolplex"> Here </a>

Project googolplex is a web server built on C++. It mainly funtions as a AI text generator, where you input the prompt, and it will return an "anwser" (actually queried from a public API). User can review their history prompts and answeres freely. 


We Constructed a CI/CD Pipeline on google cloud platform (GCP): we have detailed log info from debug all the way to fatal; test coverage report using Google Test, and code review using gerrit. We also setup a monitor dashboard to record up-time and request latency on GCP.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/demo.png" title="Demo Image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/monitor.png" title="Monitor image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     On the left, the demo screenshot of what our front-end looks like. Right, the monitor on GCP
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/coverage.jpeg" title="Coverage image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The test coverage by google test.
</div>
The server follows the NGINX standard, with REST API capabilities. It is built mostly on C++ with Boost Library (there are more easy-to-use library, but, you know, class project always want you to do in more difficult way lol).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/workflow.png" title="workflow image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The workflow of our server
</div>