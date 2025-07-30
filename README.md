# 🧠 DEPTH-ESTIMATION

This project implements a **depth estimation and segmentation pipeline** capable of analyzing a single RGB image and producing both a **dense depth map** and **object segmentation masks** based on relative distances. The model uses **DeepAnything**, a state-of-the-art deep learning model for visual understanding, and applies a **dynamic thresholding algorithm** to segment objects according to their depth in the scene.

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

