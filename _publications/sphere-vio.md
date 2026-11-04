---
title: "Sphere-VIO: Fast and Robust Visual-Inertial Odometry via Unified Spherical Representation for Wide-FoV Multi-Camera Systems"
collection: publications
category: manuscripts
permalink:  /publication/sphere-vio
excerpt: 'This work is my first PhD publication. I am the sole first author.'
date: 2026-10-29
venue: 'IEEE Robotics and Automation Letters (RAL)'
paperurl: 'https://doi.org/10.1109/LRA.2026.3748679'
citation: 'Y. Yang, Y. Xie, H. Wei, Q. Wang, B. Zhou, F. Gao, J. Ma, and J. Zhou, &quot;Sphere-VIO: Fast and Robust Visual-Inertial Odometry Via Unified Spherical Representation for Wide-FoV Multi-Camera Systems,&quot; <i>IEEE Robotics and Automation Letters</i>, doi: 10.1109/LRA.2026.3748679.'
keywords: "Cameras;Visualization;Modeling;Simultaneous localization and mapping;Measurement;Optimization;Robots;Filtering;Geometry;Timing;SLAM;Visual-Inertial SLAM;Localization"
---

**[🎬 Watch Demo Video on Bilibili](https://www.bilibili.com/video/BV1QfMF63EVA/)**

Multi-camera visual-inertial odometry (VIO) improves the robustness of visual localization by expanding the field of view. However, most existing methods are tailored for fixed camera configurations, and cannot easily support heterogeneous multi-camera systems while striking a favorable balance between tracking performance, depth estimation stability, and real-time efficiency.

To tackle these challenges, we propose Sphere-VIO, a lightweight filter-based framework centered on a unified spherical representation. It builds a unified panoramic mapping mechanism for heterogeneous multi-camera systems, paired with depth-guided cross-camera feature tracking and a low-complexity filter backend. While drastically reducing computational overhead, Sphere-VIO achieves an excellent trade-off between localization accuracy, environmental robustness, and cross-camera generality, and runs stably in real time on resource-constrained edge devices.
