---
layout: page
title: Face recognition with PCA
description: Eigenface-based face recognition in MATLAB, my first machine learning project.
importance: 8
category: undergraduate @ NIT Rourkela
---

**NIT Rourkela, summer 2017 (summer research internship)**

Under the guidance of [Dr. Anup Nandy](https://www.nitrkl.ac.in/CS/~nandya/). My first machine learning project: face recognition with principal component analysis (eigenfaces) in MATLAB, on the [AT&T Database of Faces](https://www.kaggle.com/datasets/kasikrit/att-database-of-faces) (formerly the ORL dataset) of 40 people with 10 grayscale images each.

- Each training image is flattened into a vector and centered by subtracting the mean face.
- To keep the eigendecomposition small, the covariance is computed in the low-dimensional sample space rather than the pixel space, and eigenvectors with significant eigenvalues are kept as eigenfaces.
- Training and test images are projected onto this face space, and a test image is recognized as the training image with the smallest Euclidean distance.

[Code on GitHub](https://github.com/amrit19/Facial-Recognition-using-PCA-MATLAB-Implementation)
