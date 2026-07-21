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
