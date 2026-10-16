---
layout: page
title: Human gait as a cognitive state predictor
description: Undergraduate thesis predicting cognitive state from 3D gait captured by eight Kinect sensors.
importance: 4
category: undergraduate @ NIT Rourkela
---

**NIT Rourkela, Aug 2019 to May 2020 (undergraduate thesis)**

Intelligent Computing and Computer Vision research group, advised by [Dr. Anup Nandy](https://www.nitrkl.ac.in/CS/~nandya/).

Studied whether the way a person walks reveals their cognitive state. I calibrated eight Kinect v2 sensors to reconstruct a walking person in 3D, then trained deep learning models to predict cognitive state from the reconstructed gait. EEG signals served as ground truth for cognitive state, and IMU sensors as ground truth for gait. The model explained about 95.6% of the variation in cognitive state (R² = 0.9556), suggesting that gait is a strong indicator of cognitive state. The calibration methods were published at CVIP 2021 (see [multi-Kinect camera calibration]({{ '/projects/5_kinect/' | relative_url }})).
