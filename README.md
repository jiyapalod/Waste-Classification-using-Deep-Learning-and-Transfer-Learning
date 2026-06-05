# ♻️ Waste Classification using MobileNetV2

## Overview

This project uses Deep Learning and Transfer Learning to automatically classify waste images into two categories:

- Organic Waste
- Recyclable Waste

The model is built using TensorFlow/Keras and leverages MobileNetV2 pre-trained on ImageNet for feature extraction and fine-tuning.

---

## Problem Statement

Improper waste segregation is a major environmental challenge. Manual sorting is slow, inconsistent, and prone to human error. This project aims to automate waste classification using computer vision techniques, enabling smarter waste management systems.

---

## Dataset

Source: Kaggle Waste Classification Dataset

Classes:
- Organic (O)
- Recyclable (R)

---

## Tech Stack

- Python
- TensorFlow
- Keras
- MobileNetV2
- NumPy
- Matplotlib
- Scikit-Learn

---

## Model Architecture

MobileNetV2 (Pre-trained on ImageNet)
↓
GlobalAveragePooling2D
↓
Dense(128, ReLU)
↓
Dropout(0.4)
↓
Dense(2, Softmax)

---

## Hyperparameters

| Parameter | Value |
|------------|--------|
| Input Size | 160 × 160 × 3 |
| Batch Size | 64 |
| Optimizer | Adam |
| Learning Rate | 0.0001 |
| Epochs | 10 |
| Early Stopping | Patience = 3 |
| Dropout | 0.4 |

---

## Results

### Performance

- Training Accuracy: ~94%
- Validation Accuracy: ~90%
- Validation Loss: ~0.18
- Early Stopping triggered around Epoch 6

### Classification Metrics

| Class | Precision | Recall | F1 Score |
|---------|----------|---------|----------|
| Organic | 0.97 | 0.92 | 0.95 |
| Recyclable | 0.91 | 0.97 | 0.94 |

---

## Key Features

- Transfer Learning using MobileNetV2
- Data Augmentation
- Fine-Tuning of Pre-trained Layers
- Early Stopping
- High Classification Accuracy
- Low Overfitting

---

## Future Improvements

- Multi-class waste classification
- Glass, Metal, Plastic and E-Waste categories
- Edge deployment on Raspberry Pi
- Real-time waste detection using live camera feeds

---
