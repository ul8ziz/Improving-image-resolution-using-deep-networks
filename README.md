# 📈 Image Super-Resolution Using ESRGAN

This project implements a deep learning pipeline for improving the resolution of low-quality images using ESRGAN (Enhanced Super-Resolution Generative Adversarial Network).

## 🔍 Project Overview
The goal of this project is to upscale low-resolution images (e.g., 64x64) into high-resolution versions (e.g., 256x256) using an enhanced GAN-based architecture. The system is trained on the DIV2K dataset and evaluated using PSNR and SSIM metrics.

## 🧠 Key Features
- Uses **ESRGAN** for high-quality image enhancement
- Supports early stopping during training
- Visualizes training loss over epochs
- Computes **PSNR** and **SSIM** scores to evaluate image quality
- Saves and reloads trained model weights for reuse

## 🗃️ Dataset
- **DIV2K_valid_LR_bicubic/X4** (Low-Resolution)
- **DIV2K_valid_HR** (High-Resolution)
> Images are resized to 64×64 (LR) and 256×256 (HR) for compatibility with the model.

## 📦 Requirements
```
pip install torch torchvision matplotlib pillow scikit-image tqdm
```

## 🚀 Training
```python
python train.py
```

## 💾 Model Saving
Trained models are automatically saved to:
```
../models/esrgan_generator.pth
```

## 🧪 Evaluation
Model performance is evaluated using PSNR and SSIM on test images and visual results are displayed side-by-side.

## 📁 Folder Structure
```
project/
│
├── data/                   # DIV2K dataset folders
├── models/                 # Saved ESRGAN model weights
├── train.py                # Main training script
├── inference.ipynb         # Notebook for testing the model
└── README.md
```

## 📌 License
MIT License

## 👨‍💻 Author
This project was developed as part of a master's degree research on image enhancement using deep learning.
