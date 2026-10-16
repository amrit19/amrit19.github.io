---
layout: page
title: Hand gesture password recognition
description: A dynamic hand gesture-based password system that works with an ordinary laptop webcam. ICCIS 2019.
importance: 6
category: undergraduate @ NIT Rourkela
related_publications: true
---

**NIT Rourkela, Jan 2019 to May 2019 (course project)**

A password system based on sequences of hand gestures that runs on an ordinary built-in laptop webcam instead of a Kinect camera, with no gloves or markers, so it could be added as a security layer on everyday laptops and phones. Published at ICCIS 2019.{% nocite pisipati2020gesture %}

- **Segmentation.** Each video frame is separated from its background. Three methods were compared: Otsu thresholding, a filtering and binarization pipeline, and skin-color segmentation in YCbCr space. Skin-color segmentation was the most efficient and was used for the final system.
- **Classification.** A feed-forward neural network with one hidden layer (2,500 inputs for 50×50 images, 25 hidden units and 9 outputs), trained with back-propagation and a conjugate-gradient optimizer in Octave, classifies nine gesture classes. On a 1,714-image Indian Sign Language dataset with an 80/20 split, it reached 96.16% average test accuracy.
- **Password check.** A password is a sequence of gestures with time stamps. The system unlocks only when both the recognized gestures and their timing match the stored password.
