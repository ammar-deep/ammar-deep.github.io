---
title: "3D Sensing, Pseudo-LiDAR & Autonomous Systems"
excerpt: "Multi-camera 3D perception, monocular depth-based pseudo-LiDAR, autonomous wheelchair prototype, and gesture-based human-robot interaction."
collection: portfolio
permalink: /projects/3d-sensing-autonomous/
date: 2023-06-01
---

**DeltaX.ai, Seoul — 2023–2025**

A collection of projects spanning multi-modal 3D scene understanding and autonomous system prototypes.

**3D Sensing & Pseudo-LiDAR:**

- Monocular depth estimation → 3D point cloud (pseudo-LiDAR) with dense vs sparse comparison against real LiDAR
- Multi-camera 3D object detection, tracking, static/dynamic segmentation, speed and direction estimation
- LiDAR–camera extrinsic calibration, synchronization, and multi-camera 3D reconstruction
- Real-time BEV (Bird's Eye View) and Jelly-View visualization using PyQt

**Autonomous Wheelchair POC:**

- Dual-camera (RGB + Depth) system with monocular depth for real-time obstacle distance measurement
- SLAM-based path planning with a custom panoptic segmentation model trained on Seoul urban environment data
- Enabled robust outdoor and indoor navigation for assistive mobility

**Gesture-Based Vehicle Control (HRI POC):**

- Body keypoint detection to recognize a defined gesture vocabulary
- Mapped skeletal joint inputs to mobile robot movement commands for gesture-controlled autonomous driving

**Tools & Sensors:** PyTorch · LiDAR · RGB cameras · Depth cameras · Open3D · OpenGL · PyQt · SLAM
