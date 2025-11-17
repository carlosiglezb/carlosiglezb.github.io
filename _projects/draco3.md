---
layout: page
title: Whole Body Control using Rolling Contact Joints
description: IEEE SII (2025), Frontiers in Robotics and AI (2023)
img: assets/img/draco3.png
importance: 2
category: humanoids
related_publications: true
---

<!-- Intro -->
This project consisted in the development and evaluation of our custom Whole Body Controller (WBC)including Rolling Contact Joint (RCJ) constraints. This also involved the development of our open-sourced <a href="https://github.com/UT-HCRL/rpc" target="_blank" rel="noopener noreferrer">Robot Planning and Control (RPC)</a> {% cite Bang2025RPC %} framework. This controller was evaluated in the Draco3 humanoid robot designed and built by <a href="https://apptronik.com/" target="_blank" rel="noopener noreferrer">Apptronik</a>.

<!-- Approach Overview -->
Our WBC leverages implicit hierarchies to handle tasks and enforces the RCJ via hard constraints in a Quadratic Program. This work also involved some re-design considerations at the mechanical level. In particular, the cable tensioning mechanism at the hip joint was improved to withstand longer hours of experiments and the knee motors were re-designed to allow enough power to properly carry the robot's weight. The details are provided in {% cite Bang2023 %}. Lastly, our architecture, dubbed RPC, includes several visualization and debugging tools along with multiple integrated physics engines (MuJoCo and PyBullet) to evaluate the controller prior to experiments.

Some of the experiments performed with our controller on Draco3 are shown below:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <div class="embed-responsive embed-responsive-16by9">
            {% include video.liquid path="https://www.youtube.com/embed/9qVQzY0fic8" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<div class="caption">
    Experiments of Draco3 balancing under disturbance rejection, moving sideways, squatting, balancing on one foot, and taking a step in place.
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/rpc.mp4" class="img-fluid rounded z-depth-1"  controls=true %}
    </div>
</div>

<div class="caption">
    Demo of our RPC {% cite Bang2025RPC %} framework.
</div>
