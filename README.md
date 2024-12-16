# -Wheat-Kernel-Classification-using-KNN-and-MLP-

## Overview

This project focuses on classifying a dataset of wheat kernels into three varieties: **Kama**, **Rosa**, and **Canadian**, using machine learning algorithms. The dataset consists of 210 instances, each described by seven geometric features. The primary goal is to compare the performance of the **K-Nearest Neighbors (KNN)** and **Multilayer Perceptron (MLP)** algorithms for optimal classification accuracy.

---

## Dataset Details
- **Instances**: 210
- **Classes**: Kama (70), Rosa (70), Canadian (70)
- **Attributes**:
  1. Area
  2. Perimeter
  3. Compactness (4 * π * A / P²)
  4. Kernel Length
  5. Kernel Width
  6. Asymmetry Coefficient
  7. Kernel Groove Length

---

## Methodology

### 1. **Preprocessing**
- Standardization applied to all attributes (mean = 0, variance = 1).

### 2. **Algorithms**
#### a. K-Nearest Neighbor (KNN)
- Explored different values of K (1, 3, 5).
- Performance measured using 10-fold cross-validation.
- Achieved best accuracy: **94.29%** (K=1).

#### b. Multilayer Perceptron (MLP)
- Optimized hyperparameters:
  - Learning rate: 0.5
  - Momentum: 0.2
  - Hidden layers: 6
- Achieved best accuracy: **97.14%**.

---

## Results

### Accuracy Comparison
| Algorithm | Best Configuration        | Accuracy  |
|-----------|----------------------------|-----------|
| **KNN**   | K=1                        | 94.29%    |
| **MLP**   | Learning rate=0.5, 6 layers| 97.14%    |

### Key Findings
1. **KNN**:
   - Faster computation (~0 seconds in WEKA).
   - Best suited for applications prioritizing speed.
2. **MLP**:
   - Outperformed KNN in classification accuracy and error rates.
   - Best suited for applications requiring high precision.

---

## Technologies Used
- **Algorithms**: KNN, MLP
- **Tools**: WEKA

---

## Recommendations
- Use **MLP** for scenarios where accuracy is critical.
- Use **KNN** for scenarios requiring computational efficiency.

---
