# Attention-Based CNN for Single Image Dehazing (OVAL-Net)

This project implements an end-to-end dehazing solution using the OVAL-Net architecture, specifically optimized for outdoor urban environments.

## 🛠 Features
- **Dual-Attention Mechanism:** Utilizes both Channel and Pixel attention to handle non-uniform haze.
- **Residual Learning:** Employs global residual connections to preserve image structural integrity.
- **Dataset:** Trained on the SOTS-Outdoor benchmark from the RESIDE dataset.

## 📊 Results
- **Training Loss:** ~0.063
- **Hardware:** Optimized for NVIDIA T4 GPU.
- **Interface:** Interactive Gradio UI for real-time inference.

## 🚀 How to Run
1. Open the `.ipynb` file in Google Colab.
2. Ensure you have an NVIDIA GPU runtime enabled.
3. Run all cells to launch the Gradio web interface.
