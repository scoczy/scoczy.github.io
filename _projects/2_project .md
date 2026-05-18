---
layout: page
title: A Passively Articulated Overactuated Tricopter
description: This project presents presents a passively articulated over actuated tricopter alone with a Two-Step INDI framework.
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


- A passively articulated overactuated tricopter platform is proposed.
- A two-step INDI scheme (TS-INDI) is proposed and adopted to enhance the platform’s robustness against disturbances, singularities, and actuator redundancy.
- Within the TS-INDI framework, the dynamic mismatch between thrust magnitude and direction is explicitly taken into account in a computationally lightweight manner.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_pass/statement.jpg" title="Statement" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Illustration of the thrust direction reaching the desired value faster than the thrust magnitude in the passively articulated propulsion unit.
</div>

---

## Experimental Results

### Simulation

The designed tricopter is simulated in Simscape using the proposed TS-INDI, with PID (FD allocation) and conventional INDI schemes for comparison. In simulation, the tricopter hovers at a fixed position while a linear frequency-sweep excitation (0.01–4 Hz, amplitude 2°) is injected to the pitch attitude channel, with the remaining attitude channels held at zero. Frequency-sweep experiments are performed as the pitch angle increases from 0° to 90° in 10° increments. The crossover frequency and phase margin extracted from the frequency responses are used as local measures of bandwidth and stability for comparison among three control strategies.

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_pass/chirp_line.png" title="simulation flight1" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Crossover frequency and phase margin versus attitude for the three methods. Missing entries indicate failure to complete the frequency-sweep experiment. 
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_tri/bode.png" title="simulation flight2" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Pitch-channel Bode plots at 20°, 40°, 60°, and 80° pitch; INDI cannot complete the frequency-sweep experiments beyond a pitch angle of 20°.
</div>

### Flight Test

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
