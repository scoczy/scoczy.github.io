---
layout: page
title: Over-Actuated Tricopter Platform
description: This project presents a novel over-actuated tricopter platform.
img: assets/img/proj_tri/tri.png
importance: 1
category: work
related_publications: false
---

## Overview

This project presents a novel overactuated tricopter featuring a servo-driven twisting and tilting mechanism. To address the asymmetry inherent in the tricopter configuration, we conducted a qualitative analysis of the disturbances introduced by the actuators. We emphasize the need to include gyroscopic torque effects caused by arm rotations and  proposed improved Force Decomposition (FD)-based iteration offering a low-cost computational solution.


<div class="row justify-content-sm-center">
     <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/structure.png" title="Mechanical Structure" class="img-fluid rounded z-depth-1" %}
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

- Servo-driven over-actuated omnidirectional tricopter with high maneuverability and improved flight efficiency
- Explicit modeling and evaluation of disturbances introduced by arm rotation mechanisms
- Consideration of gyroscopic torque effects caused by rotating arms, with a low-computational-cost compensation method
- Validated through simulation and real-world flight experiments

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/torque1.png" title="disturbances analysis" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Qualitative analysis of the disturbances introduced by the actuators.
</div>

---

## Experimental Results

### Simulation

The designed tricopter and the proposed FD-based Iteration (FDI) algorithm are implemented in Simscape for simulation. For comparison, the FD algorithm is also employed. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/simulation.png" title="simulation flight" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulation results of the over-actuated tricopter.
</div>

### Outdoor Flight Test

The tricopter maneuvers along a square trajectory, similar to the simulation, in an outdoor environment, with position data provided by a GPS receiver.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/outdoor.png" title="outdoor flight" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Outdoor flight results of the over-actuated tricopter.
</div>

---

## My Contributions

- Participated in the development of the over-actuated UAV platform
- Contributed to the design and implementation of flight control algorithms
- Implemented control algorithms within the PX4 autopilot framework
- Conducted flight testing, parameter tuning, and system debugging

---

## Demonstration Video
### IROS 2025 Presentation Video
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

### High-maneuverability flight demonstration
<div style="display: flex; justify-content: center; margin: 30px 0;">
  <iframe
    src="https://player.bilibili.com/player.html?bvid=BV11iD5D63Ev9&page=1"
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
