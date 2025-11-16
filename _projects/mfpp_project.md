---
layout: page
title: Multicontact Whole Body Planning
description: IEEE Humanoids 2024
img: assets/img/mfpp.png
importance: 1
category: humanoids
related_publications: true
---

<!-- Intro -->
This project focuses in our algorithm to generate dynamically feasible motions for a humanoid robot to traverse unstructured, confined spaces. As an example, we consider the case of traversing a knee knocker which requires simultaneously preserving balance and moving the robots' limbs near their kinematic limits, especially for small- and medium-size robots.

<!-- Approach Overview -->
The idea we propose is to treat the problem as a multi-particle planning problem with collision avoidance constraint. Then, we relax this nonlinear problem into a convex problem that provides kinematically feasible smooth trajectories for all of the planning frames (hands, knees, feet, torso). These paths are finally used to guide a full body trajectory optimization to verify the existence of joint plans that are dynamically feasible, i.e., respects joint angle limits, joint velocity limits, joint torque limits, and friction constraints.

A graphical video of our approach is shown below:

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/mfpp-paper-video.mp4" class="img-fluid rounded z-depth-1" controls=true %}
    </div>
</div>

The details are shown in {% cite Gonzalez2024Humanoids %} and the code is available on 
[GitHub](https://github.com/carlosiglezb/PyPnC/tree/master/pnc/planner/multicontact). 

Interactive animations of the resulting plans are available for the [G1](https://carlosiglezb.github.io/humanoids24/g1_door_crossing.html), [ergoCub](https://carlosiglezb.github.io/humanoids24/ergoCub_door_crossing.html), and [Valkyrie](https://carlosiglezb.github.io/humanoids24/valkyrie_door_crossing.html). 