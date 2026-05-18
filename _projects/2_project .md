---
layout: page
title: Over-Actuated Tricopter Platform
description: This project presents a novel over-actuated tricopter platform.
img: assets/img/proj_pass/tri_pass.png
importance: 2
category: work
related_publications: false
---

## Overview


This project presents a passively articulated over
actuated tricopter alone with a Two-Step INDI (TS-INDI)
framework. TS-INDI, built on the INDI framework, first uses Force Decomposition
(FD) to pre-allocate control increments and then distributes
the remaining increments via a pseudoinverse matrix, thereby
retaining INDI’s robustness to potential singularities and non
linearities while mitigating unbalanced propeller loads caused
by actuator redundancy. Building on this, a TS-INDI-based
extension (TS-INDI-TSM) accounts for the dynamic mismatch
between thrust magnitude and direction, improving control
performance. 

<div class="row justify-content-sm-center">
     <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_pass/structure.png" title="Mechanical Structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     (a) The proposed tilting-rotor tricopter and the defined coordinate system, where the body frame xB axis is aligned with the forward direction. (b) Structural details of the 2-DOF joint. (c)Photograph of a 2-DOF joint.(d) The geometric dimensions of the tricopter.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_pass/Control.png" title="Control Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Hierarchical TS-INDI control framework of the overactuated tricopter.
</div>

---

## Technical Highlights


- A passively articulated overactuated tricopter platform is proposed. It adopts a centralized architecture, enabling flight without reliance on external infrastructure.
- An INDI-based control framework is adopted to enhance the platform’s robustness to disturbances and singularities. To explicitly handle actuator redundancy, a two-step INDI scheme (TS-INDI) is proposed by
integrating Force Decomposition (FD) into the INDI framework, thereby avoiding secondary null-space objectives and eliminating dependence on motor thrust at specific operating points.
- Within the TS-INDI framework, the dynamic mismatch between thrust magnitude and direction is explicitly taken into account in a computationally lightweight manner, improving allocation accuracy and thereby
enhancing the achievable phase margin.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_pass/statement.jpg" title="Statement" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Hierarchical TS-INDI control framework of the overactuated tricopter.
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

<div style="display: flex; justify-content: center; margin: 30px 0;">
  <div style="width: 100%; max-width: 720px; aspect-ratio: 16 / 9;">
    <iframe
      src="https://player.bilibili.com/player.html?bvid=BV1i6cXzfEMk&page=1"
      style="width: 100%; height: 100%;"
      frameborder="no"
      allowfullscreen="true">
    </iframe>
  </div>
</div>

---
