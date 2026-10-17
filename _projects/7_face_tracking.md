---
layout: page
title: Face detection and tracking
description: Real-time face tracking with Viola-Jones detection and Arduino-controlled pan and tilt servos.
importance: 7
category: undergraduate @ NIT Rourkela
---

**[NIT Rourkela](https://www.nitrkl.ac.in/), Aug 2018 to Dec 2018 (Product Development Lab)**

A real-time system that follows a person's face with a regular webcam and two servo motors.

- **Detection.** MATLAB grabs 320×240 frames from the webcam and finds the face with a Viola-Jones cascade detector.
- **Control.** The center of the detected face is sent over a serial link to an Arduino, which compares it with the middle of the frame and steps a pan servo and a tilt servo to follow the face.
- **Tracking.** Once a face is found, the system can switch to histogram-based CAMShift tracking on the hue channel, which follows the face without running the detector on every frame.

[Code on GitHub](https://github.com/amrit19/Facial-Detection-and-Tracking-System-using-Arduino)
