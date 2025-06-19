# 🧠 Brain_Tumor_Detection
This project uses the YOLOv8 (You Only Look Once, Version 8) deep learning model to detect and localize brain tumors in medical imaging (e.g., MRI scans). Leveraging the speed and accuracy of YOLOv8, our model identifies tumor regions in real-time with bounding boxes. The goal is to provide a fast and accurate computer-aided diagnosis (CAD) system that identifies the presence and location of brain tumors using deep learning.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Project Workflow](#project-workflow)
- [Dataset](#dataset)
- [Installation](#installation)
- [Training](#training)
- [Inference](#inference)
- [Results](#results)
- [Requirements](#requirements)

---

## 📖 Overview

**YOLOv8** (You Only Look Once version 8) is the latest version of the popular object detection architecture developed by **Ultralytics**. It improves detection accuracy and speed over its predecessors.

In this project:
- MRI images of the brain are used.
- Tumors are detected and localized using bounding boxes.
- Model performance is visualized using annotated outputs.
- The complete pipeline is implemented using the Ultralytics YOLOv8 Python package.

---

## 🔁 Project Workflow

```mermaid
graph TD
    A[Data Collection] --> B[Data Annotation (YOLO Format)]
    B --> C[Train-Test Split]
    C --> D[Model Configuration (YOLOv8)]
    D --> E[Training with Ultralytics]
    E --> F[Evaluation and Metrics]
    F --> G[Inference on New Images]
    G --> H[Visualization and Interpretation]
```
## 📂 Dataset
The dataset contains MRI brain images with corresponding annotations for tumor regions.

Format: Images (.jpg or .png) and annotations in YOLO format (.txt)

Classes: 0 for Tumor

Folder structure:
└── dataset/
    ├── images/
    │   ├── train/
    │   ├── val/
    └── labels/
        ├── train/
        ├── val/

---
## ⚙️ Installation
1. Clone the repository
```
git clone https://github.com/your-username/brain-tumor-detection-yolov8.git
cd brain-tumor-detection-yolov8
```
2. Create and activate a virtual environment (optional)
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. Install dependencies
```
pip install -r requirements.txt
```

---

### ✅ Requirements
All dependencies are managed via pip. Ensure you have:

Python ≥ 3.8

pip ≥ 20.0

CUDA (optional, for GPU acceleration)

---

### 🙌 Acknowledgements
Ultralytics YOLOv8

Roboflow for data preparation tools

Public datasets used: https://universe.roboflow.com/123-qdx85/road-damage-detection-yjqzv.
