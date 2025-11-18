---
layout: page
title: Exokeleton Development
description: IHMC Quix and Eva
img: assets/img/hyq-balancing.jpeg
importance: 1
category: exoskeletons
related_publications: true
---

<!-- Intro -->
While working at the 
<a href="https://robots.ihmc.us/" target="_blank" rel="noopener noreferrer">Institute for Human and Machine Cognition (IHMC)</a>, I contributed to two exoskeleton projects:  <a href="https://www.ihmc.us/exoskeleton-for-improving-mobility/" target="_blank" rel="noopener noreferrer">Quix</a> and <a href="https://robots.ihmc.us/exoskeletons-for-augmenting-human-performance" target="_blank" rel="noopener noreferrer">Eva</a>.


<!-- Quix Overview -->
Quix is an assisstive exoskeleton designed and built by IHMC.
In the Quix project, I mostly helped with the evaluation and testing of the finished exoskeleton in preparation for the Cybathlon competition, where we obtained the 4th palce. The details of the mechanical design and the controller are shown in {% cite Peterson2022 %}. A video of the competition summary is shown below:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <div class="embed-responsive embed-responsive-16by9">
            {% include video.liquid path="https://www.youtube.com/embde/mIbaOjXYxHs" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<div class="caption">
    Highlights form the Cybathlon 2020 competition.
</div>

<!-- Eva Overview -->
Eva is an augmentative exoskeleton designed and built by IHMC.
In the Eva project, I largely contributed to the initial bringup of the software-hardware integration of the robot. This entailed setting up the motors and tunning the motor controller communicating over CAN and connecting these to our software controller stack (now, <a href="https://github.com/ihmcrobotics/simulation-construction-set-2" target="_blank" rel="noopener noreferrer"> SCS2</a>). The sensors that were integrated were encoders and pressure sensors initially mounted on the soul of the foot. The current version of Eva is available on <a href="https://robots.ihmc.us/exoskeletons-for-augmenting-human-performance" target="_blank" rel="noopener noreferrer">IHMC's Eva section</a>.