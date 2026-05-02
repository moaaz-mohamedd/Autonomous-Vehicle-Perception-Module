# Phase 1 - Classical Machine Learning for Image Classification

## Overview

This phase focuses on applying classical machine learning techniques to image classification as an early step in the Autonomous Vehicle Perception Module project.

The goal was to build baseline models before moving into deep learning approaches in Phase 2.

In this phase, we tested different classical ML models using raw pixel features and PCA-reduced features, then compared their performance based on accuracy, macro F1-score, and training time.

---

## Dataset

**Dataset:** CIFAR-10  
**Task:** Image Classification  
**Image Type:** RGB Images  
**Phase Focus:** Classical Machine Learning Baselines

The images were processed and converted into numerical feature vectors to make them suitable for traditional machine learning models.

---

## Main Steps

- Loaded and explored the dataset
- Analyzed image samples and class distribution
- Converted images into feature vectors
- Tested models using raw pixel features
- Applied PCA for dimensionality reduction
- Trained multiple classical ML models
- Compared models using accuracy, macro F1-score, and execution time

---

## Models Used

The following models were tested:

- KNN Baseline
- Gaussian Naive Bayes
- KNN with PCA
- Random Forest
- Bagging Classifier
- AdaBoost Classifier

---

## Results

| Model | Features | PCA Components | Accuracy | Macro F1 | Time (Seconds) |
|---|---|---:|---:|---:|---:|
| Random Forest | PCA Features | 100 | 41.73% | 41.09% | 19.77 |
| Bagging Classifier | PCA Features | 100 | 37.07% | 36.68% | 54.05 |
| KNN + PCA | PCA Features | 50 | 33.13% | 32.77% | 0.27 |
| AdaBoost Classifier | PCA Features | 100 | 32.23% | 31.53% | 31.44 |
| KNN + PCA | PCA Features | 100 | 31.07% | 30.16% | 0.38 |
| Gaussian Naive Bayes | Raw Pixels | No | 30.27% | 27.66% | 1.24 |
| KNN + PCA | PCA Features | 200 | 29.80% | 28.39% | 0.54 |
| KNN Baseline | Raw Pixels | No | 28.93% | 26.94% | 6.20 |

---

## Best Model

The best-performing model in Phase 1 was:

Random Forest with PCA Features

**Key Observations:**

Random Forest achieved the best overall performance among the tested classical machine learning models.
PCA helped reduce the feature space and improved the performance of some models.
KNN with PCA was much faster than the raw pixel KNN baseline.
Bagging achieved the second-best accuracy but required the highest execution time.
Gaussian Naive Bayes was fast, but its performance was limited on image data.
Classical machine learning models gave useful baselines, but their performance was limited compared to deep learning methods.