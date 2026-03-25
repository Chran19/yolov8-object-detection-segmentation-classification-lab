# YOLOv8 Object Detection, Segmentation & Classification Lab

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-orange.svg)](https://github.com/ultralytics/ultralytics)
[![Deep Learning](https://img.shields.io/badge/Deep%20Learning-Computer%20Vision-blue.svg)](#)

**📚 Course:** Deep Learning Lab (2311332L)  
**🎓 Institution:** MIT Academy of Engineering  
**📍 Department:** Computer Engineering (Software Engineering)  
**📅 Academic Year:** 2025-26  
**🏫 Batch:** A1, A2, A3

**Repository:** [https://github.com/Chran19/yolov8-object-detection-segmentation-classification-lab](https://github.com/Chran19/yolov8-object-detection-segmentation-classification-lab)

---

## 📋 Project Overview

This is a comprehensive deep learning laboratory project implementing **YOLOv8** for three fundamental computer vision tasks:

1. **Object Detection** — Localizing and classifying objects with bounding boxes
2. **Instance Segmentation** — Pixel-level segmentation masks for detected objects
3. **Image Classification** — Single-label classification on ImageNet dataset

The project demonstrates the complete machine learning pipeline including data preparation, model training, evaluation, hyperparameter tuning, multi-model benchmarking, and model export for deployment.

---

## �‍💼 Course Faculty

| Role                  | Name             |
| --------------------- | ---------------- |
| **Course Instructor** | Dr. Dipti Ghusse |
| **Project Guide**     | Dr. Dipti Ghusse |

---

## 👥 Group Members

| Roll Number  | Name                       |
| ------------ | -------------------------- |
| 202301100007 | Yashwardhan Jangid         |
| 202301100032 | Shreyash Kumbhar           |
| 202301100046 | Ranjeet Choudhary (Leader) |
| 202301100047 | Rishabh Rai                |

---

## 🏗️ Project Structure

```
yolov8-object-detection-segmentation-classification-lab/
├── YOLOv8_YOLO_Assignment.ipynb          # Main notebook (42 cells)
├── README.md                              # Project documentation
├── .gitignore                             # Git ignore rules
├── Custom_Images/
│   ├── Girraafe.jpg                       # Sample image 1
│   └── Leaders.jpg                        # Sample image 2
└── Detection_Results/                      # Output directory for saved results
```

---

## 📚 Notebook Structure (13 Sections)

The Jupyter notebook contains 42 cells organized into the following sections:

| #   | Section                                   | Description                                              |
| --- | ----------------------------------------- | -------------------------------------------------------- |
| 1   | Title & Header                            | Project gradient header with branding                    |
| 2   | Project Group Details                     | Institute, course, faculty, and group member information |
| 3   | Undertaking / Declaration                 | Academic integrity commitment                            |
| 4   | Environment & Dependencies                | Package installation and environment setup               |
| 5   | Dataset Preparation                       | COCO128 dataset loading and exploratory analysis         |
| 6   | Object Detection                          | Model loading, training, evaluation, and inference       |
| 7   | Instance Segmentation                     | YOLOv8-seg model with mask visualization                 |
| 8   | Image Classification                      | YOLOv8-cls model with Top-5 predictions                  |
| 9   | Multi-Model Benchmarking                  | Performance comparison (yolov8n vs yolov8s vs yolov8m)   |
| 10  | Fine-Tuning & Hyperparameter Optimization | 3 experimental configurations with data augmentation     |
| 11  | Model Export & Deployment                 | Export to ONNX and TorchScript formats                   |
| 12  | Real-World Applications                   | Domain-specific detection demo                           |
| 13  | Results Summary & Custom Testing          | Metrics summary and custom image inference               |

---

## � Tech Stack

| Component         | Library             | Version |
| ----------------- | ------------------- | ------- |
| Framework         | Ultralytics YOLOv8  | 8.2.0   |
| Deep Learning     | PyTorch             | 2.11.0  |
| Computer Vision   | OpenCV              | Latest  |
| Data Processing   | NumPy, Pandas       | Latest  |
| Visualization     | Matplotlib, Seaborn | Latest  |
| Model Supervision | Supervision         | Latest  |
| Language          | Python              | 3.10+   |

---

## 🚀 Getting Started

### Prerequisites

Ensure Python 3.10+ is installed. Create a virtual environment:

```bash
python -m venv .venv
.venv\Scripts\activate  # Windows
source .venv/bin/activate  # Linux/Mac
```

### Installation

Install all dependencies:

```bash
pip install ultralytics==8.2.0 opencv-python pandas numpy matplotlib seaborn supervision pyyaml h5py roboflow
```

### Running the Notebook

1. Clone the repository:

```bash
git clone https://github.com/Chran19/yolov8-object-detection-segmentation-classification-lab
cd yolov8-object-detection-segmentation-classification-lab
```

2. Activate virtual environment and launch Jupyter:

```bash
jupyter notebook YOLOv8_YOLO_Assignment.ipynb
```

3. Run cells sequentially from top to bottom

### Custom Image Testing

Place your images in the `Custom_Images/` folder:

- `Girraafe.jpg` — Image 1 for detection testing
- `Leaders.jpg` — Image 2 for detection testing

Run the custom image cells in Section 13 to see side-by-side original vs. detected results.

---

## 📈 Key Features

- ✅ **Three Vision Tasks** — Detection, Segmentation, Classification in one notebook
- ✅ **Multi-Model Architecture** — Base, Small, and Medium variants comparison
- ✅ **Data Augmentation** — HSV, rotation, translation, scaling, mosaic, mixup
- ✅ **Hyperparameter Tuning** — Grid search experiments
- ✅ **Model Export** — ONNX and TorchScript formats
- ✅ **PyTorch Compatibility** — Safe weight loading for PyTorch 2.6+
- ✅ **Visualization** — Side-by-side detection comparisons, confusion matrices, training curves
- ✅ **Custom Images** — Direct inference on local images with confidence scores

---

## 🔬 Methodology

### 1. Data Preparation

- COCO128 dataset auto-download
- Class name parsing and EDA
- 12-image grid visualization

### 2. Model Training

- YOLOv8n Base detection model
- Training on COCO128 for 10 epochs
- Augmentation pipeline (HSV, rotation, flip, scale, mosaic, mixup)
- Momentum-based SGD optimization

### 3. Evaluation

- Confusion matrix generation
- Precision, recall, F1-score per class
- Training/validation curve analysis
- mAP@50 and mAP@50-95 metrics

### 4. Task-Specific Models

- **Detection:** YOLOv8n-detect
- **Segmentation:** YOLOv8n-seg with mask overlay
- **Classification:** YOLOv8n-cls with Top-5 predictions

### 5. Benchmarking

- Speed comparison (yolov8n vs yolov8s vs yolov8m)
- Parameter count analysis
- Inference time measurements

### 6. Export & Deployment

- ONNX format export with dynamic input support
- TorchScript format for PyTorch deployment
- Dual format with independent error handling

---

## � Expected Results

### Detection Performance

- **Model:** YOLOv8n (nano)
- **Dataset:** COCO128 (80 classes)
- **Inference Time:** ~30-50ms (CPU)
- **mAP@50:** Comparable to Ultralytics baseline

### Custom Image Results

- **Girraafe.jpg:** Animal detection (giraffe, zebras, etc.)
- **Leaders.jpg:** Person detection (22+ individuals with confidence scores)

### Export Formats

- ✅ **ONNX** — Cross-platform deployment
- ✅ **TorchScript** — PyTorch production deployment

---

## 📁 Dataset Details

### COCO128

- **Total Images:** 128 annotated training images
- **Classes:** 80 object categories (persons, vehicles, animals, objects, etc.)
- **Format:** Pascal VOC and COCO JSON formats
- **Size:** ~3 MB (compact for quick prototyping)
- **Source:** Microsoft COCO 2017 subset via Ultralytics

---

## 🎯 Learning Objectives

By completing this lab, students will:

- ✅ Understand YOLOv8 architecture and variants
- ✅ Implement detection, segmentation, and classification pipelines
- ✅ Apply data augmentation for improved model generalization
- ✅ Perform hyperparameter optimization via grid search
- ✅ Analyze model performance with confusion matrices and metrics
- ✅ Compare multi-model performance trade-offs (accuracy vs. speed)
- ✅ Export models for production deployment (ONNX, TorchScript)
- ✅ Run custom inference on local images

---

## 🔍 Troubleshooting

### PyTorch Weight Loading Issues

The notebook includes a `safe_load` wrapper for PyTorch 2.6+ compatibility:

```python
torch.load = safe_load  # Handles weights_only parameter
```

### CUDA/GPU Support

The notebook supports CPU-only mode (default) or CUDA if available:

```python
device = 0 if torch.cuda.is_available() else 'cpu'
```

### Dataset Download Failures

If COCO128 doesn't download, the notebook falls back to pre-trained weights for inference demonstration.

---

## 📚 References

- **YOLOv8 Documentation:** https://docs.ultralytics.com/
- **PyTorch:** https://pytorch.org/
- **OpenCV:** https://opencv.org/
- **COCO Dataset:** https://cocodataset.org/

---

## 📄 License

This project is developed as part of the **Deep Learning Lab (2311332L)** course at MIT Academy of Engineering, Computer Engineering Department.

**Academic Year:** 2025-26 | **Batches:** A1, A2, A3

---

_Developed with ❤️ by Group Members: Yashwardhan Jangid, Shreyash Kumbhar, Ranjeet Choudhary, Rishabh Rai_

**Last Updated:** March 25, 2026
