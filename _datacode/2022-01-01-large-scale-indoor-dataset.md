---
title: "A large scale dataset for indoor visual localization with high precise ground truth"
excerpt: "We present a challenging new dataset for indoor localization research. We have recorded the whole internal structure of Fengtai Wanda Plaza which is over 15800 square meters area with a Navvis M6 device. The dataset contains 679 RGBD panoramas and 2664 query images collected by three different smartphones. In addition to the data, aligned 3D point cloud is produced after the elimination of moving objects based on the building floorplan. Furthermore, a method is provided to generate corresponding high resolution depth images for each panorama. By fixing the smartphones on the device using a specially designed bracket, 6 degree of freedom camera poses can be calculated precisely. We believe it can give a new benchmark for indoor visual localization. <br/><img src='/images/datacode/navvis-m6-device.png' width='500'>"
collection: datacode
---

## A large scale dataset for indoor visual localization with high precise ground truth

We present a challenging new dataset for indoor localization research. We have recorded the whole internal structure of Fengtai Wanda Plaza which is over 15800 square meters area with a Navvis M6 device. The dataset contains 679 RGBD panoramas and 2664 query images collected by three different smartphones. In addition to the data, aligned 3D point cloud is produced after the elimination of moving objects based on the building floorplan. Furthermore, a method is provided to generate corresponding high resolution depth images for each panorama. By fixing the smartphones on the device using a specially designed bracket, 6 degree of freedom camera poses can be calculated precisely. We believe it can give a new benchmark for indoor visual localization.

Fig.1(a) is the Navvis M6 device used for data collection. It is equipped with six high-resolution cameras(b) for capturing 360° images. The device has one Velodyne VLP-16 LiDAR mounted on the top reaching up to 100 meters and three single-line LiDARs reaching up to 30 meters. The device can produce RGB panorama at a resolution of 8192x4096 and depth panorama at a resolution of 1024x512. Note that the device provides both dense and sparse depth images at the same resolution. Besides, an IMU sensor is fixed inside the head of the device to calculate the trajectory and some anchor points(c) are deployed on the ground evenly in the building to modify the trajectory estimation. The position of these anchor points is measured by a real-time kinematic measurement system. The query images are captured by three different types of smartphones which are HUAWEI honor10, mate8 and mate9(d). To fix these smartphones on the device, a bracket is 3D-printed.

<div align='center'>
  <img src="/images/datacode/navvis-m6-device.png" width="400">
  <br>Fig.1 Navvis M6
</div>

## Data Collections

The dataset includes two dataset: training dataset and query dataset. For conveniently downloading the dataset, we divide the dataset into six parts according to the plaza floor. Each part has the same file structure.

### (1)Data format

#### (a) RGB images

All RGB images are stored as JPG files in unrectified 8-bit format. The structure of the dataset is shown in Fig.2. The panoramas are saved in ##pano## folder and named as ##<scan_number>-pano.jpg## with image size of 8192x4096, where ##<scan_number>## is the sequence number of scan points in the trajectory. 36 perspective images are extracted from each panorama and saved in image folder. The query images are saved in another folder named by the phone as it can be seen in Fig.3.

<div align='center'>
  <img src="/images/datacode/indoor-database-structure.png" width="400">
  <br>Fig. 2 Database file structure
</div>

<div align='center'>
  <img src="/images/datacode/indoor-query-structure" width="400">
  <br>Fig.3 Query file structure
</div>

#### (b) Depth images

The depth images contain depth value in millimeters are stored as lossless-compressed PNG files in unrectified 16-bit format. ##pano_depth## contains depth information of each visual panorama with the size of 8192x4096. ##image_depth## contains depth image of each perspective image.

#### (c) Point clouds

Point cloud is saved as ##pointcloud.ply## with point density less than 5mm. The file contains 10 parameters each point, which is (x, y, z, r, g, b, norm x, norm y, norm z, curv). The (x,y,z) are the 3D Cartesian coordinates of the point with respect to the world coordinate and the color information is saved in triplets of (r,g,b). For each point, its normal vector and curvature are recorded as the last four elements, which are critical criterion when determining the visibility of the point in specific perspective.

#### (d) Pose

The pose information consists of 3D location vector and quaternion. The pose iunformation of one trajectory is saved in a YAML document file: ##pos.yml##. Note that the reference coordinate of the pose information is the world coordinate system.

### (2)Training dataset

[download]

### (3)Query dataset

[download]

## Development tools

We provide a set of development kits written in C++ code on the website for users to manipulate the dataset. The code provides functions to produce transformation matrix from camera coordinate to the world coordinate and 3D positions of the feature points.

##transformation matrix generation##: The function ##Quat2Dcm()## is used to produce transformation matrix from camera coordinate to the world coordinate based on rotation vector in the form of quaternions and translation vector.

##3D position generation##: The function ##Pixel2Point()## is used to calculate the 3D position of feature points in the world coordinate based on corresponding depth information and transformation matrix.

### Reference
Yuchen Liu, **Wei Gao\***, Zhanyi Hu. A large-scale dataset for indoor visual localization with high-precision ground truth. The International Journal of Robotics Research, 41(2), pp. 129-135, 2022.

### Contact

If you want to download the above databases, please contact me.