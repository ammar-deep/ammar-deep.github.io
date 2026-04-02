---
title: "Smart Factory Vision & Edge AI Deployment"
excerpt: "27-camera smart factory intrusion and defect detection system, road anomaly detection, gaze estimation, and model deployment on Jetson, TI, and Hailo hardware."
collection: portfolio
permalink: /projects/smart-factory-edge-ai/
date: 2023-09-01
---

**DeltaX.ai, Seoul — 2023–2025**

Industrial vision systems have a way of making you care deeply about things that barely matter in research — frame rate, memory footprint, what happens when one camera in a rack of 27 drops its stream at 3am.

The smart factory project was the largest system I built at DeltaX: 27 cameras, RTSP streams, human intrusion detection and product defect detection, all running at 25 FPS in C++. Getting it working once was straightforward; getting it to run stably over days and weeks without intervention was the real problem. Camera recovery logic, stream management, alert thresholds that don't fire on every shadow passing through frame.

The road anomaly work was on the opposite end of the scale but had its own tight constraints: pothole and crack detection with oriented bounding boxes, exported to ONNX, running on a Hailo AI accelerator. Small model, strict latency budget, no GPU in sight.

The gaze estimation project is probably the best example of the kind of optimization work nobody talks about but everyone eventually has to do. I took an existing GPU-based pipeline (L2CS-Net), converted it entirely to ONNX, swapped out the face detector for something lighter and compatible, rewrote the inference path, and landed at 8–12 FPS on CPU-only hardware. Not glamorous, but it runs in deployment contexts where a discrete GPU simply isn't available.

More broadly, a large part of working on edge AI at DeltaX was this last-mile problem: taking a model that performs well in training and making it actually usable on Jetson, TI, or Hailo hardware through quantization, distillation, and TensorRT/DeepStream pipeline integration.

**Stack:** PyTorch · C++ · ONNX · TensorRT · DeepStream · NVIDIA Jetson · TI Board · Hailo · OpenCV
