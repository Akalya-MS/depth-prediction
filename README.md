# depth-prediction
Depth Estimation Using MiDaS and U-Net
Overview
This repository features a monocular depth estimation framework that integrates MiDaS and U-Net to produce precise depth maps. Depth estimation is essential in several computer vision domains, such as robotics, autonomous driving, and augmented reality. By combining MiDaS and U-Net, the model enhances depth prediction accuracy while remaining optimized for real-time execution.

Features
Hybrid Pipeline: The approach leverages MiDaS for initial depth prediction, followed by U-Net for refinement, improving the clarity and accuracy of depth maps.
Dataset Training: The model is trained and validated on the KITTI dataset, a widely recognized benchmark for depth estimation research.
High Precision: The MiDaS + U-Net combination achieves a 96% accuracy rate on the preprocessed dataset.
Edge Device Compatibility: Designed for efficient deployment on edge AI hardware, maintaining a compact model size of 10MB.
Real-time Execution: The architecture supports fast inference speeds, making it well-suited for real-time depth estimation applications.
Model Architecture
The depth estimation pipeline consists of the following key components:

MiDaS Preprocessing: MiDaS generates an initial depth estimation from a single image, providing a coarse depth map.
U-Net Enhancement: The MiDaS output is refined using a U-Net model, which preserves local details and improves overall depth accuracy.
Training Process: The U-Net model is trained on a curated subset of KITTI, incorporating image normalization, data augmentation, and optimized loss functions for superior performance.
Deployment Optimization: The final model is optimized for Edge AI hardware, ensuring a balance between computational efficiency and prediction accuracy.
