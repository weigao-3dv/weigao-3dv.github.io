---
title: "Boosting image-based localization via randomly geometric data augmentation"
excerpt: "<img src="/images/research/2020 Boosting image-based.PNG" width="500">"
collection: research
---

<div align='center'>
  <img src="/images/research/2020 Boosting image-based.PNG" width="500">  
</div>

## Abstract

Visual localization is a fundamental problem in computer vision and robotics. Recently, deep learning has shown to be effective for robust monocular localization. Most deep learning-based methods utilize convolution neural network (CNN) to regress global 6 degree-of-freedom (Dof) pose. However, these methods suffer from pose sparsity, leading to over-fitting during training and poor localization performance on unseen data. In this paper, we try to alleviate this issue by implementing randomly geometric augmentation (RGA) during training. Specifically, we firstly estimate the depth map using a depth estimation network for the initial training image. Combing the estimated depth, RGB image and its corresponding pose, we can randomly synthesize new images of different views. The synthesized and initial images are used to train the pose regression network. Experiment results show our geometric augmentation strategy can significantly improve the localization accuracy.

## Reference

Yiming Wan, **Wei Gao\***, Sheng Han, Yihong Wu. Boosting image-based localization via randomly geometric data augmentation. Abu Dhabi National Exhibition Center (ADNEC), Abu Dhabi, United Arab Emirates (UAE), 10.25-10.28, 688-692, ICIP 2020. [**DOI**](https://doi.org/10.1109/ICIP40778.2020.9190809)