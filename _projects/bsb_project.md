---
layout: page
title: Sensitivity in Multicontact Balance Stability Boundary
description: ASME-JMR (2018), ASME-IDETC (2018), ASME-IDETC (2017)
img: assets/img/darwin-bsb.png
importance: 3
category: humanoids
related_publications: true
---

<!-- Intro -->
In this project, I studied the quantitative impact of the variability in torque limits and variability in contact area in the ability of a robot to remain in balance.

<!-- Approach Overview -->
This study builds on the concept of Balance Stability Boundary (BSB) is introduced in {% cite Mummolo2017ASME %} and applied to a humanoid in more detail in {% cite Mummolo2018 %}. The BSB is an area in the Center of Mass (CoM) state-space that determines if a robot is in balance at any given time based on the current contact configuration.
The BSB looks as shown below for a humanoid robot in single support (left) and double-support phase.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/bsb-ss.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/bsb-ds.png" class="img-fluid rounded z-depth-1" %}
    </div>    
</div>


This is computed numerically by solving an optimization problem at many different CoM positions and looking for a feasible trajectory that brings the CoM to a statically stable position (e.g., the center of the feet). This renders the BSB numerically challenging to compute, so it is computed offline. What happens if we wanted to know what this BSB would have looked like if we had stronger motors, or larger feet, or a different contact configuration? One would need to recompute the corresponding BSB. Instead, in this project I show that one can use the Sensitivity Theorem from optimal control theory to iniexpensively compute an estimate of the BSB within small bounds of perturbing the torque or contact limits {% cite Gonzalez2018ASME %}. Below is what the BSB looks like as we increase the torque limits.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/publication_preview/BSB.png" class="img-fluid rounded z-depth-1" %}
    </div>    
</div>

<div class="caption">
    As the torque limits increase, the BSB grows until it reaches a point of saturartion, i.e., stronger motors will not make the robot more stable. This is because at this point the foot will start tipping and become more unstable.
</div>

I showed that it is possible to analytically determine when the BSB saturates under torque limit variation. In the case of variability of the area of the base of support, one can estimate when this saturation is reached.