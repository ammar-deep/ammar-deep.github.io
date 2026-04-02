---
title: "Smart Factory Vision & Edge AI Deployment"
excerpt: "27-camera smart factory intrusion and defect detection system, road anomaly detection, gaze estimation, and model deployment on Jetson, TI, and Hailo hardware."
collection: portfolio
permalink: /projects/smart-factory-edge-ai/
date: 2023-09-01
---

**DeltaX.ai, Seoul — 2023–2025**

Production-level edge AI systems and factory automation projects demanding real-time inference on constrained hardware.

**Smart Factory Monitoring:**

- Built a 27-camera RTSP-based human intrusion and product defect detection system running at 25 FPS in C++
- Multi-camera synchronization, stream management, and alert integration

**Road Anomaly Detection (Edge):**

- Pothole and crack detection using oriented bounding box (OBB) models
- ONNX export and deployment on Hailo AI accelerator via onnxruntime

**Gaze Estimation (CPU Optimization):**

- Converted GPU-based L2CS-Net gaze estimation pipeline to a fully ONNX-based CPU solution
- Replaced RetinaFace with a lightweight ONNX-compatible face detector
- Achieved 8–12 FPS real-time gaze estimation on CPU-only hardware
- Packaged as a PyTorch-free Python module for easy cross-platform deployment

**Edge AI Deployment (general):**

- Model optimization via quantization (INT8/FP16) and knowledge distillation for Jetson, TI, and Hailo boards
- TensorRT and DeepStream pipeline integration for real-time multi-model inference

**Tools:** PyTorch · C++ · ONNX · TensorRT · DeepStream · NVIDIA Jetson · TI Board · Hailo · OpenCV
