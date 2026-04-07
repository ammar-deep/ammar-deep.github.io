---
title: "3D Sensing, Pseudo-LiDAR & Autonomous Systems"
excerpt: "Multi-camera 3D perception, monocular depth-based pseudo-LiDAR, autonomous wheelchair prototype, and gesture-based human-robot interaction."
collection: portfolio
permalink: /projects/3d-sensing-autonomous/
date: 2023-06-01
status: completed
organization: DeltaX.ai, Seoul
period: 2023 – 2025
tech: "LiDAR, Pseudo-LiDAR, Monocular Depth, 3D Detection, SLAM, Autonomous Wheelchair, HRI"
header:
  teaser: images/pub_placeholder.png
---

**DeltaX.ai, Seoul — 2023–2025**

Some of the most interesting work I did at DeltaX didn't have a clean product brief — it was more "can we actually do this, and is it good enough to be useful?" A lot of the 3D sensing work started there.

The pseudo-LiDAR project came from a practical question: real LiDAR is expensive, so what do you actually lose by using monocular depth to generate a point cloud instead? I built a pipeline to compare the two side by side — dense vs sparse, structured vs noisy — running in real time with a PyQt interface so you could watch the difference directly. The honest answer is "it depends on your application," but working through why taught me a lot about where depth estimation actually breaks down.

The multi-camera perception work was more involved: extrinsic calibration and time synchronization across cameras, 3D object detection and tracking, static/dynamic segmentation, speed and direction estimation. BEV and Jelly-View visualization on top of everything, which sounds optional until you've tried to debug a 3D tracker without it.

The autonomous wheelchair was a POC but a genuinely challenging one. Dual cameras (RGB + depth), SLAM-based path planning, and a custom panoptic segmentation model we trained on data collected in Seoul — outdoors, in environments that hadn't been mapped in advance. That last part was the hard bit.

The gesture control project was simpler but fun. Detect body keypoints, define a gesture vocabulary, map joint movements to robot commands. The interesting engineering problem was making the recognition robust enough that the robot didn't start moving every time the driver adjusted their grip.

**Stack:** PyTorch · LiDAR · RGB cameras · Depth cameras · Open3D · OpenGL · PyQt · SLAM
