---
title: "Bidirectional Trajectory Computation for Odometer-Aided Visual-Inertial SLAM"
excerpt: "<img src="/images/research/2021 Bidirectional Trajectory.PNG" width="500">"
collection: research
---

<div align='center'>
  <img src="/images/research/2021 Bidirectional Trajectory.PNG" width="500">  
</div>

## Abstract

Odometer-aided visual-inertial SLAM systems typically have a good performance for navigation of wheeled platforms, while they usually suffer from degenerate cases before the first turning. In this paper, firstly we perform an observability analysis w.r.t. the extrinsic parameters before the first turning, which is a complement of the existing results of observability analyses. Secondly, inspired by the above observability analyses, we propose a bidirectional trajectory computation method, by which the poses before the first turning are refined in the backward computation thread, and the real-time trajectory is adjusted accordingly. Experimental results prove that our proposed method not only solves the problem of the unobservability of accelerometer bias and extrinsic parameters before the first turning, but also results in more accurate trajectories in comparison with the state-of-the-art approaches.

## Reference

Jinxu Liu, **Wei Gao\***, Zhanyi Hu. Bidirectional Trajectory Computation for Odometer-Aided Visual-Inertial SLAM. in IEEE Robotics and Automation Letters, vol. 6, no. 2, pp. 1670-1677, April 2021. [**DOI**](https://doi.org/10.1109/LRA.2021.3059564)