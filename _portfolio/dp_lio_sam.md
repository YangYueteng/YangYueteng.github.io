---
title: "DP-LIO-SAM: Dual-LiDAR SLAM with Multi-Plane Constraints"
excerpt: "Video of the Undergraduate thesis project "
collection: portfolio
---

<a href="https://www.bilibili.com/video/BV1AV4y1C77S/" target="_blank" 
   style="display:block; position:relative; width:100%; max-width: 720px; margin: 0 auto 1.5rem auto; padding-top:56.25%; overflow:hidden; border-radius:6px; border:1px solid #eaeaea;">
<iframe src="//player.bilibili.com/player.html?bvid=BV1AV4y1C77S&page=1" 
        scrolling="no" 
        border="0" 
        frameborder="no" 
        framespacing="0" 
        allowfullscreen="true" 
        style="position:absolute; top:0; left:0; width:100%; height:100%; pointer-events:none;">
</iframe>
</a>

<p style="font-size: 0.9rem; color: #666; text-align:center; margin-top: -1rem; margin-bottom: 1.5rem;">
👆 Click the window to open the full video on Bilibili (new tab)
</p>

### Project Overview
This work is my undergraduate final thesis project. I developed **DP-LIO-SAM**, a dual-LiDAR mapping and localization system enhanced by multi-plane constraints. The framework is built upon the classic LIO-SAM pipeline, with targeted optimizations for robust and accurate LiDAR-inertial odometry in complex urban environments.

### Key Improvements
Based on the original LIO-SAM framework, I made the following modifications:
1.  **Dual-LiDAR Calibration & Fusion**: Implemented point cloud stitching and data fusion for two LiDAR sensors to expand the effective field of view.
2.  **Wheel Odometry Integration**: Incorporated wheel speed odometry measurements to further stabilize motion estimation.
3.  **Scan Context Loop Closure**: Added a Scan-Context-based loop closure detection module, referencing the design of SC-LIO-SAM, to correct accumulated long-term drift.
4.  **Plane Adjustment with π-Posegraph**: Reproduced the Plane Adjustment algorithm from the 2021 ICRA paper *π-LSAM*, and constructed a π-posegraph factor graph that establishes constraints between plane features and robot poses, as well as between consecutive poses.
5.  **Efficient Plane Optimization**: Designed a plane filtering mechanism and applied marginalization to plane parameter variables, significantly accelerating the Bundle Adjustment process.

### Demo Highlights
This demo tests DP-LIO-SAM on the **KAIST Urban08 dataset** (from the publication *Complex Urban LiDAR Data Set*), and is played back at 10× speed from a run on a Dell laptop.
- The visualized point clouds correspond to planar features extracted for the Plane Adjustment module. They are dominated by static urban landmarks, with dynamic objects such as moving vehicles filtered out.
- Close-up views at loop closure segments demonstrate the trajectory optimization effect after loop closure factors are added.
- The top-left panel of the video shows the full 3D mapping result of the system.
