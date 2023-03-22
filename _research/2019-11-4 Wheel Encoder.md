---
title: "Visual-Inertial Odometry Tightly Coupled with Wheel Encoder Adopting Robust Initialization and Online Extrinsic Calibration"
excerpt: "<img src='/images/research/2019 Wheel Encoder.PNG' width='500'>"
collection: research
---

<div align='center'>
  <img src="/images/research/2019 Wheel Encoder.PNG" width="500">  
</div>

## Abstract

Combining camera, IMU and wheel encoder is a wise choice for car positioning because of the low cost and complementarity of the sensors. We propose a novel extended visual-inertial odometry algorithm tightly fusing data from the above three sensors. Firstly we propose an IMU-odometer pre-integration approach utilizing complete IMU measurements and wheel encoder readings, to make scale estimation more accurate in subsequent 4-degrees of freedom (DoF) optimization. Secondly we develop an original initialization module where encoder readings are fully utilized to refine gravity direction and provide an initial value for camera pose in real scale. Thirdly, we design a computationally efficient online extrinsic calibration method by fixing the linearization point for the rotational component of IMU-odometer extrinsic parameters, which is deployed depending on the convergence of accelerometer bias. Experimental results prove the robustness of our initialization module and the accuracy of the whole trajectory, as well as the improvement brought about by online extrinsic calibration. Our program can also run on an Nvidia Jetson TX2 module in real time.

## Reference

Jinxu Liu, **Wei Gao\***, Zhanyi Hu. Visual-Inertial Odometry Tightly Coupled with Wheel Encoder Adopting Robust Initialization and Online Extrinsic Calibration. IROS, THE VENETIAN MACAO, MACAU, CHINA, 11.4 - 11.8, pp. 5391-5397, 2019. [**DOI**](https://doi.org/10.1109/IROS40897.2019.8967607)