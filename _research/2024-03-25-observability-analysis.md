---
title: "Implementation and observability analysis of visual-inertial-wheel odometry with robust initialization and online extrinsic calibration"
excerpt: "Combining camera, IMU and wheel encoder is a wise choice for car positioning because of the low cost and complementarity of the sensors. We propose a novel extended visual-inertial odometry algorithm based on sliding window tightly fusing data from the above three sensors. Firstly we propose an IMU-odometer pre-integration approach utilizing complete IMU [**Read More**] <br/><img src='/images/research/2024-observability-analysis.png' width='500'>"
collection: research
---

<div align='center'>
  <img src="/images/research/2024-observability-analysis.png" width="500">  
</div>

## Abstract

Combining camera, IMU and wheel encoder is a wise choice for car positioning because of the low cost and complementarity of the sensors. We propose a novel extended visual-inertial odometry algorithm based on sliding window tightly fusing data from the above three sensors. Firstly we propose an IMU-odometer pre-integration approach utilizing complete IMU measurements and wheel encoder readings, to make scale estimation more accurate in subsequent 4-degrees of freedom (DoF) optimization. Secondly we develop an original initialization module where encoder readings are fully utilized to refine gravity direction and provide an initial value for camera pose in real scale. Thirdly, we design a computationally efficient online extrinsic calibration method by fixing the linearization point for the rotational component of IMU-odometer extrinsic parameters, which is deployed depending on the convergence of accelerometer bias. Fourthly, we give an observability analysis of our optimization based approach under more general assumption. Extensive experiments are performed on two sets of data in various scenes, bringing the state-of-the-art visual odometry and visual-inertial odometry algorithms into comparison. Experimental results prove the overwhelmingly better performance of our proposed approach on the above two sets of data, as well as the robustness of our initialization module and the improvement resulted from online extrinsic calibration.


## Reference

Jinxu Liu, **Wei Gao\***, Chuyun Xie, Zhanyi Hu. Implementation and observability analysis of visual-inertial-wheel odometry with robust initialization and online extrinsic calibration. Robotics and Autonomous Systems, vol. 176, 104686, June 2024. [**DOI**](https://doi.org/10.1016/j.robot.2024.104686)