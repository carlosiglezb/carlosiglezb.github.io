---
layout: page
title: Design and Integration of Person Carrying Robot
description: ASME-IDETC (2023)
img: assets/img/bumpybot.jpg
importance: 1
category: mobile base
related_publications: true
---

<!-- Intro -->
The goal for this project was to build a mobile robot that could carry a person and navigate autonomously. 

<!-- Approach Overview -->
Starting almost from scratch, I chose the sensors, computers, and servo drives for the robot. I chose EtherCAT as the communication protocol to achieve realtime speeds with high bandwidth and integrated it into the ROS ecosystem to easily integrate off-the-shelf sensors (e.g., Lidar and cameras). Moreover, I used ros-control to seemlesly transition from simulation in Gazebo to real robot experiments. I open-sourced my code on <a href="https://github.com/carlosiglezb/bumpybot" target="_blank" rel="noopener noreferrer">GitHub</a> and provide design and implementation details in {% cite Gonzalez2023ASME %}.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/bumpybot-move-up.gif" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/bumpybot-move-right.gif" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/bumpybot-move-down.gif" class="img-fluid rounded z-depth-1" %}
    </div>    
</div>

<div class="caption">
    First prototype as we tested moving in straight lines: up, right, and down.
</div>
