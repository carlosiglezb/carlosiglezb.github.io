---
layout: page
title: Balance Control of Robots with Point Feet
description: IROS 2020
img: assets/img/hyq-balancing.jpeg
importance: 1
category: quadrupeds
related_publications: true
---

<!-- Intro -->
This project applies the balance theory development by 
<a href="https://royfeatherstone.org/" target="_blank" rel="noopener noreferrer">Prof. Roy Featherstone</a> to a quadruped robot balancing on two point feet in 3D space.

<!-- Approach Overview -->
The proposed strategy consists in constructing a kinematic equivalence between the quadruped robot balancing on two point-feet in 3D space, and an underactuated inverted pendulum balancing on a 2D plane. An angular-based balance control law is designed for the virtual underactuated inverted pendulum, and the resulting momentum is translated to the quadruped through the aforementioned kinematic map. This is paired with a control framework known as the Reactive Controller Framework (RCF) to achieve both balance and locomotion on two point-feet. This is showcased in the challenging task resembling tightrope walking.

The following video shows the results of our balance controller {% cite Gonzalez2020IROS %}:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <div class="embed-responsive embed-responsive-16by9">
            {% include video.liquid path="https://www.youtube.com/embed/Cun1OBJXsUo" class="img-fluid rounded z-depth-1" %}
        </div>
    </div>
</div>

<div class="caption">
    Physical experiments of balance controller on HyQ and simulations showing versatility to also perform line walking locomotion.
</div>
