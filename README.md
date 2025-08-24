# 🧠 Brain MRI Analysis Suite

> A modular deep learning project for Brain Tumor Classification & Segmentation with Streamlit UI
---

## 📌 Overview

This project provides an end-to-end brain MRI analysis system:

Tumor Classification → Classifies MRIs into categories (e.g., No Tumor, Pituitary, etc.)

Tumor Segmentation → Generates precise tumor masks from MRI scans

Streamlit App → Interactive interface for classification, segmentation & visualization

Built using PyTorch, Streamlit, and OpenCV, the system is modularized for easy training, inference, and deployment.
---

## 📂 Project Structure
- ├── segmentation_dataset/            # Phase 2 data
- │   └── Patient_xxx/...
- ├── classification/                  # Phase 1 data
- │   └── no_tumor/, glioma/, ...
- ├── models/                          # Model definitions
- │   ├── unet_attention.py
- │   └── resnet_classifier.py
- ├── train/                           # Training scripts
- │   ├── train_segmentation.py
- │   └── train_classification.py
- ├── inference/                       # Inference + utils
- │   ├── predict_class.py
- │   ├── gradcam.py
- │   ├── predict_segmentation.py
- │   └── visualization.py
- ├── utils/                           # Helpers (dataset loaders, etc.)
- │   ├── dataloader_classification.py
- │   ├── dataloader_segmentation.py
- │   └── transforms.py
- ├── app.py                           # Streamlit app

---

## ⚙️ Features

- ✔️ Tumor Classification using ResNet-based CNN
- ✔️ Tumor Segmentation with Attention U-Net
- ✔️ Interactive Streamlit UI for uploading & analyzing scans
- ✔️ Grad-CAM visualization for interpretability
- ✔️ Modular training/inference pipeline

---
## 🚀 Getting Started
- **1️⃣ Clone Repo**
- 
```bash
git clone https://github.com/<your-username>/brain-mri-analysis.git
cd brain-mri-analysis
```

- **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

- **3️⃣ Run Streamlit App**
```bash
streamlit run app.py
```

---

## 📊 Datasets

Classification Dataset → MRI images in 4 folders (No Tumor, Pituitary, Meningioma, Glioma)

Segmentation Dataset → Patient-wise folders containing MRI scans & corresponding tumor masks

_⚠️ Due to size constraints, datasets are not included in this repo. Please download and place them in the respective folders._

---

## 🎯 Future Work

Add cloud hosting (Streamlit Cloud / Hugging Face Spaces)

Expand dataset support (more modalities)

Integrate explainable AI modules beyond Grad-CAM

---

# 👨‍💻 Author

Ved Khajone
Driven by Curiosity.....
---

