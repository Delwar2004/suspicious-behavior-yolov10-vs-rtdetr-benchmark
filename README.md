# 🚀 YOLOv10n vs RT-DETR: A Benchmark Study for Suspicious Behavior Object Detection

<p align="center">

![Python](https://img.shields.io/badge/Python-3.12-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red)
![Ultralytics](https://img.shields.io/badge/Ultralytics-YOLOv10-success)
![RT-DETR](https://img.shields.io/badge/RT--DETR-Object%20Detection-orange)
![License](https://img.shields.io/badge/License-MIT-green)

</p>

---

## 📌 Project Overview

This repository presents an experimental benchmark study comparing **YOLOv10n** and **RT-DETR** for suspicious behavior object detection.

The primary objective of this work is **not to develop a production-ready detection system**, but to conduct a structured comparative analysis of two modern object detection architectures under identical experimental conditions.

This benchmark serves as a preliminary investigation for a larger research project in intelligent surveillance and vision-based behavior understanding.

---

## 🎯 Objectives

- Benchmark YOLOv10n and RT-DETR on the same dataset
- Compare detection performance using standard object detection metrics
- Analyze the strengths and limitations of each architecture
- Establish a baseline for future research

---

## 📂 Dataset

The benchmark was conducted using a custom suspicious behavior detection dataset containing four semantic categories:

- Suspicious
- Fight
- Normal
- Poster

Dataset Statistics

| Split | Images |
|--------|--------:|
| Train | 1,688 |
| Validation | 161 |
| Test | 80 |

---

## 🏗️ Models Evaluated

### YOLOv10n

- One-stage object detector
- Lightweight architecture
- Optimized for real-time inference

### RT-DETR

- Transformer-based object detector
- End-to-end detection framework
- Focused on high detection accuracy

---

## ⚙️ Experimental Configuration

- Framework: Ultralytics
- Python 3.12
- PyTorch 2.x
- Image Size: 640×640
- Optimizer: AdamW (Auto)
- GPU: NVIDIA Tesla T4
- Mixed Precision (AMP): Enabled

---

## 📊 Evaluation Metrics

The models were evaluated using standard object detection metrics:

- mAP@50
- Precision
- Recall
- F1-score

---

## 🏆 Benchmark Results

| Rank | Model | mAP@50 | Precision | Recall | F1-score |
|------|--------|--------:|----------:|--------:|----------:|
| 🥇 | RT-DETR | **0.9455** | 0.9093 | **0.9615** | **0.9340** |
| 🥈 | YOLOv10n | 0.9255 | **0.9189** | 0.9130 | 0.9159 |

---

## 🔍 Key Findings

- RT-DETR achieved the highest overall detection performance.
- YOLOv10n demonstrated slightly higher precision.
- RT-DETR achieved better recall and F1-score, indicating stronger overall detection capability.
- The benchmark highlights the trade-off between lightweight one-stage detectors and transformer-based architectures.

---

## 📁 Repository Structure

```text
YOLOv10-vs-RTDETR-Benchmark/
│
├── notebook/
│   └── SuspiciousBehavior_YOLOv10n_RTDETR.ipynb
│
├── results/
│   ├── YOLOv10_results.csv
│   ├── RTDETR_results.csv
│   └── Final_Model_Comparison.csv
│
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```
---

## 🚀 Future Work

This benchmark represents an initial experimental study.

Future research directions include:

- Evaluation on larger surveillance datasets
- Cross-dataset generalization
- Lightweight deployment for edge devices
- Real-time video inference
- Multi-camera surveillance systems
- Human behavior understanding with Vision-Language Models

---

## ⚠️ Disclaimer

This repository is intended for educational and research benchmarking purposes.

The experiments were conducted to compare object detection architectures and should not be interpreted as a production-ready surveillance solution.

---

## 👨‍💻 Author

**MD DELWAR HUSEN**

Undergraduate Student  
Information and Communication Engineering (ICE)

Machine Learning • Deep Learning • Computer Vision • Medical AI

---

⭐ If you found this project useful, consider giving the repository a star.
