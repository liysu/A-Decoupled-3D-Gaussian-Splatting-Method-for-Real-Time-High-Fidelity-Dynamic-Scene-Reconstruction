# A Decoupled 3D Gaussian Splatting Method for Real-Time High-Fidelity Dynamic Scene Reconstruction

![Demo Animation](assets/demo.gif)

## Overview

In the recent years, Neural Radiance Fields (NeRF) have emerged as an efficient and photorealistic solution for the implicit reconstruction of three-dimensional (3D) scenes from a limited set of two-dimensional(2D) images. In addition, 3D Gaussian Splatting (3DGS) has significantly improved the rendering quality and speed through explicit representations. However, the reconstruction of dynamic scenes remains a significant challenge. To address this issue, we propose an innovative framework for the real-time reconstruction and rendering of dynamic scenes. First, we uncouple the dynamic and static regions based on local geometric variations and adaptively determine the optimal segmentation threshold in a data-driven manner according to a dynamic score. Next, we reconstruct the static regions using the conventional 3D Gaussian approach. Finally, for the dynamic regions, we introduce a deformation field with a motion-consistency constraint to enforce spatiotemporal continuity in the motion trajectories of the dynamic Gaussians. Results of extensive experiments demonstrate that the proposed method achieves higher rendering quality and faster rendering speed than other existing methods.

## Results

### Comparison with Baseline Methods

| Ground Truth | 4D GAUSSIAN | NeRF Player | Ours |
|:------------:|:-----------:|:-----------:|:----:|
| ![GT](assets/GT.gif) | ![4D GAUSSIAN](assets/4D%20GAUSSIAN-.gif) | ![NeRF Player](assets/nerf%20player-.gif) | ![Ours](assets/ours-.gif) |

*Figure: Qualitative comparison with baseline methods on dynamic scene reconstruction*
