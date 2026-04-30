# Phase 2 - Deep Learning for Traffic Sign Recognition

## Overview

This phase focuses on applying deep learning techniques for traffic sign recognition using the **German Traffic Sign Recognition Benchmark (GTSRB)**.

The goal was to build and compare different deep learning approaches for traffic sign classification, image reconstruction, transfer learning, learning rate scheduling, and CNN feature visualization.

---

## Dataset

**Dataset:** German Traffic Sign Recognition Benchmark (GTSRB)  
**Number of Classes:** 43  
**Image Size:** 32x32x3  
**Task:** Traffic Sign Classification

Dataset split:

| Split | Samples |
|---|---:|
| Training | 31,367 |
| Validation | 7,842 |
| Testing | 12,630 |

---

## Notebooks

| File | Description |
|---|---|
| `Phase2.ipynb` | CNN, optimizer comparison, AutoEncoder, and VGG16 transfer learning |
| `Part4.ipynb` | Learning rate scheduler comparison using PyTorch |
| `part5.ipynb` | CNN feature map visualization |

---

## Methods Used

- CNN model for traffic sign classification
- Data augmentation
- Optimizer comparison
- AutoEncoder for image reconstruction
- Transfer Learning using VGG16
- Learning rate scheduler comparison
- CNN feature map visualization

---

## Best Results

| Experiment | Best Method | Best Accuracy |
|---|---|---:|
| Baseline CNN | Custom CNN | 91.72% test accuracy |
| Optimizer Comparison | CNN with SGD | 95.23% test accuracy |
| Transfer Learning | VGG16 | 91.50% test accuracy |
| Scheduler Comparison | CosineAnnealingLR | 99.94% validation accuracy |

---

## Highest Accuracy Achieved

The highest accuracy achieved in this phase was:

```text
99.94% validation accuracy

PyTorch CNN + CosineAnnealingLR Scheduler

95.23% test accuracy

TensorFlow CNN with SGD optimizer