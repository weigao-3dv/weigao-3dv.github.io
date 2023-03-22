---
title: "Dynamic object-aware monocular visual odometry with local and global information aggregation"
excerpt: "In this paper, we present a deep learning-based approach to monocular visual odometry. We propose a LCGR(Local Convolution and Global RNN) module which utilizes several independent 3D convolution layers to filter noise from features extracted by FlowNet, as well as to model local information, and a Bi-ConvLSTM layer to [**Read More**]<br/><img src='/images/research/2020 Dynamic object-aware.PNG' width='500'>"
collection: research
---

<div align='center'>
  <img src="/images/research/2020 Dynamic object-aware.PNG" width="500">  
</div>

## Abstract

In this paper, we present a deep learning-based approach to monocular visual odometry. We propose a LCGR(Local Convolution and Global RNN) module which utilizes several independent 3D convolution layers to filter noise from features extracted by FlowNet, as well as to model local information, and a Bi-ConvLSTM layer to model time series and capture global information. In addition, our network jointly predicts optical flow as an auxiliary task by measuring photometric consistency in a self-supervised way to help the encoder for better motion feature extraction. In order to alleviate the effects of non-Lambertian surfaces and dynamical objects in the scene, a confidence mask layer is estimated and epipolar constraint is added to the training process. Experiment results indicate competitive performance of the proposed framework to the state-of-art methods.

## Reference

Yiming Wan, **Wei Gao\***, Sheng Han, Yihong Wu. Dynamic object-aware monocular visual odometry with local and global information aggregation. Abu Dhabi National Exhibition Center (ADNEC), Abu Dhabi, United Arab Emirates (UAE), 10.25-10.28, 603-607, ICIP 2020. [**DOI**](https://doi.org/10.1109/ICIP40778.2020.9190930)