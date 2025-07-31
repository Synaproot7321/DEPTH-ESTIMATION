# 🧠 DEPTH-ESTIMATION

<p align="justify">
This project implements a <strong>depth estimation and segmentation pipeline</strong> capable of analyzing a single RGB image and producing both a <strong>dense depth map</strong> and <strong>object segmentation masks</strong> based on relative distances. The model uses <strong>DeepAnything</strong>, a state-of-the-art deep learning model for visual understanding, and applies a <strong>dynamic thresholding algorithm</strong> to segment objects according to their depth in the scene.
</p>

---

## 🎯 Objective

To estimate the **depth of objects from a single image** (without requiring stereo vision or special sensors) and **automatically segment them** by analyzing spatial relationships, with robustness to lighting variation, shadows, and occlusion.

This system is useful in scenarios where hardware constraints prevent the use of 3D cameras or stereo setups, such as:

- Mobile devices
- Drones and UAVs
- Real-time industrial monitoring
- Autonomous navigation prototypes

---

## 🌟 Key Features

- 📷 **Single Image Input**  
  No need for depth sensors or stereo pairs — works with any RGB image.

- 🧠 **DeepAnything Integration**  
  Leverages a robust pre-trained vision transformer (ViT) to extract scene-level features and produce high-resolution depth maps.

- 🧮 **Dynamic Segmentation via Adaptive Thresholds**  
  Segments foreground objects using depth distribution statistics (e.g., median, quantiles) to automatically distinguish regions of interest.

- ⚙️ **Modular Architecture**  
  The pipeline is cleanly separated into modules for inference, thresholding, visualization, and export.

- 📈 **Customizable Output**  
  Generates grayscale depth maps, heatmaps, binary masks, and composite overlays.

---

## 🛠️ Technologies Used

- `Python 3.10`
- `PyTorch` 
- `OpenCV` 
- `NumPy` 
- `Matplotlib` 
- `DeepAnything` 

---

## 🖼️ Output Example (Visual)

Below is a sample of the OCR result shown directly over the input image, highlighting the recognized text areas:

<div align="center">
  <img src="https://github.com/user-attachments/assets/ddd22d99-4567-490c-a9c5-7680ab651843" alt="OCR Output Sample" width="700"/>
  <p><em>This image shows how the algorithm inferred and segmented objects from the original image.</em></p>
</div>

## 📊 Impact

This depth estimation algorithm brings value in various computer vision applications, particularly where specialized hardware like depth sensors is not available:

- 🧠 **Improved Scene Understanding**  
  Enables systems to infer spatial relationships between objects using only a single image.

- 🎯 **Supports Object Segmentation and Tracking**  
  Enhances the ability to isolate and analyze objects based on their depth, improving downstream tasks like detection or monitoring.

- ⚙️ **Hardware-Efficient**  
  Offers a software-based alternative to stereo cameras or LiDAR, reducing costs and complexity.

- 🛠️ **Versatile Applications**  
  Useful in robotics, quality control, and autonomous systems that require depth perception with minimal sensor input.

> This model makes depth-aware vision more accessible in environments with limited resources or hardware constraints.

