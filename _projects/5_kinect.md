---
layout: page
title: Multi-Kinect camera calibration
description: Pairwise and octagonal calibration methods for eight Kinect v2 sensors. CVIP 2021.
importance: 5
category: undergraduate @ NIT Rourkela
related_publications: true
---

**NIT Rourkela, May 2018 to Jan 2020**

Developed two methods for calibrating eight Microsoft Kinect v2 sensors, as the 3D capture setup for my [undergraduate thesis]({{ '/projects/4_gait/' | relative_url }}). The first is pairwise calibration: consecutive pairs of Kinects view a 3D object on a treadmill, and calibration runs in six steps, from pre-calibration and image capture through exporting camera parameters, generating live point clouds and matching them, to checking the merged point cloud. The second is simultaneous single-camera calibration of all eight cameras on the same setup with a novel octagonal model. The two methods reached overall mean reprojection errors of 1.37 and 0.42 pixels, with best cases of 0.63 and 0.27 pixels, and outperformed existing techniques on both root mean square and reprojection error {% cite hazra2021kinect %}.

This built on earlier work in the summer of 2018 in the Machine Intelligence and Bio-Motion Laboratory, extracting people from Kinect v2 video with [adaptive background subtraction](https://github.com/amrit19/Extracting-Object-from-Video-using-Adaptive-Background-Subtraction).
