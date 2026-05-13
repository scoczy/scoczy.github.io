---
layout: page
title: Over-Actuated Tricopter Platform
description: This project presents a novel over-actuated tricopter platform.
img: assets/img/proj_tri/tri.png
importance: 1
category: work
related_publications: true
---

## Overview

This project presents a novel overactuated tricopter featuring a servo-driven twisting and tilting mechanism. To address the asymmetry inherent in the tricopter configuration, we conducted a qualitative analysis of the disturbances introduced by the actuators. We emphasize the need to include gyroscopic torque effects caused by arm rotations and  proposed improved Force Decomposition (FD)-based iteration offering a low-cost computational solution.


<div class="row justify-content-sm-center">
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/structure.png" title="Mechanical Structure" class="img-fluid rounded z-depth-1" %}
    </div>
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/torque.png" title="Asymmetry Inherent" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Configuration of the proposed tilt-rotor tricopter.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/Control.png" title="Control Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overall control architecture of the over-actuated tricopter.
</div>

---

## Technical Highlights

---

## Experimental Results

### Simulation

The designed tricopter and the proposed FD-based Iteration (FDI) algorithm are implemented in Simscape for simulation. For comparison, the FD algorithm is also employed. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/simulation.png" title="Control Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulation results of the over-actuated tricopter.
</div>

### Outdoor Flight Test

The tricopter maneuvers along a square trajectory, similar to the simulation, in an outdoor environment, with position data provided by a GPS receiver.



---

## My Contributions

- UAV flight control
- Over-actuated aerial vehicles
- Fault-tolerant control
- Autonomous aerial robotics
- Control allocation and robust control

---

## Demonstration Video
- IROS 2025 Presentation Video
<div style="display: flex; justify-content: center; margin: 30px 0;">
  <iframe
    src="https://player.bilibili.com/player.html?bvid=BV1EQqGBoEnG&page=1"
    width="960"
    height="540"
    scrolling="no"
    border="0"
    frameborder="no"
    framespacing="0"
    allowfullscreen="true">
  </iframe>
</div>

---
