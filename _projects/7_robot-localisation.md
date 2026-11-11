---
layout: page
title: Robot localisation and sensor fusion
description: Uncertainty-aware odometry and visual, inertial and kinematic fusion for robots.
img: assets/img/publication_preview/UVO.png
importance: 7
category: robotics and perception
permalink: /projects/robot-localisation/
---

**Role:** Researcher, ARAS Labs, 2018 to 2022. I worked in a seven-person team spanning mechanical, control, electronics and mechatronics engineering. This includes my MSc thesis on cable-robot localisation.

### Deep odometry with uncertainty

[A Consistency-Based Loss for Deep Odometry Through Uncertainty Propagation](https://arxiv.org/abs/2107.00366) (ICRA 2023) propagates pose uncertainty to balance incremental and trajectory-level losses. It improves pose accuracy and provides uncertainty estimates for localisation.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/publication_preview/UVO.png" title="Deep odometry with uncertainty propagation" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

### Localising cable-driven robots

- I fused position and orientation estimates from camera and inertial sensors with uncertainty-aware robot kinematics.
- With another engineer, I designed and implemented pose estimation for each sensor array. We also designed and built the robot's end effector, data-acquisition system and joints.
- [Graph-Based Visual-Kinematic Fusion and Monte Carlo Initialization for Fast-Deployable Cable-Driven Robots](https://doi.org/10.1109/IROS55552.2023.10342316) (IROS 2023) localises and calibrates cable-driven robots jointly, using factor graphs and Monte Carlo initialisation.

<div class="row justify-content-sm-center">
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/publication_preview/calib.png" title="Calibrating a deployable cable-driven robot" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/publication_preview/arasiref.png" title="ARAS-IREF pose-estimation framework" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

### Other perception work

- I proposed an uncertainty-aware localisation subsystem for long-term and short-term odometry in autonomous-vehicle navigation.
- [ARAS-IREF](https://ieeexplore.ieee.org/document/9071852) (ICRoM 2019, Best Paper Award) is an inexpensive, open-source infrared pose-reference system.
- [ARC-Net](https://arxiv.org/abs/2007.03063) (ICMLA 2020) fuses data from several inertial sensors with capsule networks for activity recognition. [Code](https://github.com/hamed-d/ARC-Net)
