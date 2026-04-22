# Attention-Based CNN for Single Image Dehazing (OVAL-Net)

[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1F5383GNsJ2eRkNZueHDsqR9RbwhGzgAv#scrollTo=34e0703b)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Framework: PyTorch](https://img.shields.io/badge/Framework-PyTorch-orange.svg)](https://pytorch.org/)

This repository contains the implementation of **OVAL-Net**, a high-performance convolutional neural network designed for single image dehazing. By leveraging a dual-attention mechanism, this model effectively restores clarity in complex outdoor urban environments where haze density is non-uniform.

---

## 📥 Pre-trained Weights
The serialized model tensors (`.pth` file) exceed GitHub's standard file size limitations for direct uploads.

* **Download Link:** [Download OVAL-Net Weights (Google Drive)](https://drive.google.com/file/d/1aYGzxudR69He8SWqmTH9t4fiTY3WGxva/view?usp=drive_link)
* **Setup:** Place the downloaded `.pth` file in the root directory of this project to enable the inference engine.

---

## 🧠 Architecture Overview
OVAL-Net replaces traditional physics-based scattering models with a deep-learning end-to-end approach focused on two key pillars:

1. **Dual-Attention Mechanism:**
    * **Channel Attention (CA):** Recalibrates feature maps to correct spectral distortions and color shifts.
    * **Pixel Attention (PA):** Assigns higher weights to spatially distant regions where haze is densest.
2. **Global Residual Learning:** The network learns the "haze residue" rather than reconstructing the clear image from scratch, preserving fine structural textures through identity mapping.

---

## 🧪 Experimental Results
The model was trained and validated on the **SOTS-Outdoor (RESIDE)** benchmark.

* **Convergence:** Achieved a final L1 Training Loss of **0.0632** within 5 refinement epochs.
* **Optimization:** Fully optimized for **NVIDIA T4 GPUs** using **Automatic Mixed Precision (AMP)**.
* **Inference:** Real-time restoration capability via an integrated Gradio web interface.

---

## 🚀 Getting Started

### Prerequisites
* Python 3.8+
* PyTorch / Torchvision
* Gradio (for the interactive UI)
* CUDA-enabled GPU

### Usage
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/anuradhapaswan1/Attention-Based-Single-Image-Dehazing.git](https://github.com/anuradhapaswan1/Attention-Based-Single-Image-Dehazing.git)



