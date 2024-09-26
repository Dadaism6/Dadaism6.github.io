---
layout: page
title: UCLA Structure-Computer Interaction Lab                
description: Undergraduate Researcher
img: assets/img/robot.jpg
importance: 2
category: research
---
2020.6 - 2022.6

I spend the majority of my undergraudate research passions at <a href="https://structures.computer">UCLA Structure-Computer Interaction Lab</a> I mainly work on two sub-project.     

<h3>Low-Cost Autonomous Weed-Control Agri-Robot Project</h3>

Our goal is to built an agricultural robot that can freely navigate thrwo the crops and perform weed-control. This seeminly easy task actually requires complex design. The most difficulty thing is: how to help the robot navigate through the crops, while maintaining the low cost? 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/robot_real.jpg" title="real robot" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/robot.jpg" title="ideal robot" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Our robot
</div>

The first thing we tried is LiDAR ("light detection and ranging") sensor. LiDAR is commonly used for today's autonomous driving. However, the 3D LiDAR sensor is way too expensive for agri-robot. Instead, we use 2D sensor. Thus, we need to differentiate from a 2D data the "roads" we want. We developed a robotic navigation algorithm for road identification system and improved the navigation accuracy by 30% (compared with mutli-Ransac  and Pearl ) for the robot while maintained at low cost.

We also built an back-up plan: vision. Using Yolo-v5, I trained from scratch a model that can identify the flax, and then build a algorithms that find flax lines from it. Then, we can easily get the destination we want.

I also built a simulation environment using Gazebo (then using Unreal Engine) and ROS to test the robotic navigation algorithm easier.

<div class="row">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/touchSide.png" title="Lidar Image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.html path="assets/img/flax.jpg" title="Vision image" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.html path="assets/img/simenv.png" title="Simulation Env image" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>
<div class="caption">
     On the left, the demo for the LiDAR method. Top right, the demo for the vision method. Bottom right, the simulation environment using Unreal Engine 4.
</div>


<h3>Soft Robot Project</h3>
The second project I involved is the soft robot project. By the time I joined the lab, the robot has already been designed. The things left to be solved is more about physics: how long/tall/big should we build the robot to achieve certain speed? While given the physical dimensions and sizes of the robot, it is easy to get the maximum theoritical speed, it is hard to go in the reversed direction.

I develop a inverse design model that are able to generate parameters given the desired velocity. The design consist of two part: forward training and backward optimization. The purpose of forward training is to create a simulating model that functions the same as our simulator. We use simple fully-connected network and an improved loss function for the forward training. For the backward optimization, we freeze the pre-trained forwarding model and treate the parameters as the weight and optimize it. We apply further constrains to the parameters so that it follows the basic physic laws.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/softrobot.png" title="soft robot" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Our soft robot
</div>
