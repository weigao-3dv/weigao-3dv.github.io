---
title: "BSP-MonoLoc: Basic Semantic Primitives Based Monocular Localization on Roads"
excerpt: "<img src='/images/research/2021 BSP-MonoLoc.PNG' width='500'>"
collection: research
---

<div align='center'>
  <img src="/images/research/2021 BSP-MonoLoc.PNG" width="500">  
</div>

## Abstract

Robust visual localization in traffic scenes is a fundamental problem for self-driving vehicles. However, it is still challenging to achieve accurate localization performance because of drastic viewpoint and illumination changes. To address the issues, we design a novel monocular localization framework based on a light-weight prior map, called BSP-MonoLoc, which leverages the 2D semantic primitives from the monocular images and the 3D basic semantic primitives from the prior map. These primitives are commonly available but lack of distinctive signature. To effectively make associations between the 2D and 3D primitives and refine the vehicle’s pose, we adopt an iterative optimization method, where an efficient hierarchical sample strategy is designed to give a good initial prediction for the associations and the pose. Experimental results on the KAIST dataset and our dataset demonstrate the proposed method can achieve high localization accuracy and run at a real-time performance.

## Reference

Heping Li*, Changliang Xue, Feng Wen, Hongbo Zhang, **Wei Gao**. BSP-MonoLoc: Basic Semantic Primitives Based Monocular Localization on Roads. 2021 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2021),  Prague, Czech Republic, 9.27-10.01, IROS 2021. [**DOI**](https://doi.org/10.1109/IROS51168.2021.9636321)