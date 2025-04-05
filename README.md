# 🧠 Breast Cancer Classification – Logistic Regression from Scratch (No ML Libraries)

This project implements a **logistic regression algorithm from scratch using only NumPy**, without relying on machine learning libraries like PyTorch or TensorFlow. The goal is to classify **breast cancer diagnoses** (Benign vs. Malignant) based on medical and demographic data.

---

## 🩺 Project Description

Breast cancer is one of the most common forms of cancer among women globally. Early and accurate diagnosis is essential to improving treatment outcomes. In this project, we use a real dataset to train a logistic regression classifier to distinguish between **benign (non-cancerous)** and **malignant (cancerous)** tumors.

---

## 📁 Dataset Overview

The dataset includes the following features:

- `Age`: Patient's age
- `Menopause`: Menopausal status (0: post, 1: pre)
- `Tumor size`: Tumor size in cm
- `Involved nodes`: Presence of metastatic axillary lymph nodes (1: present, 0: absent)
- `Breast`: Cancer spread (1: spread, 0: not spread)
- `Metastatic`: Cancer metastasis
- `Breast quadrant`: Location in the breast
- `History`: Family or personal history of cancer (1: yes, 0: no)
- `Diagnosis result`: Target variable (Benign or Malignant)

---

## ✅ Key Features & Tasks

### 1️⃣ Data Preprocessing
- Loaded the dataset and removed rows with missing values  
  *(optional: predicted missing values for extra credit)*
- Converted categorical/string fields into numerical values
- Normalized numerical features for better convergence

### 2️⃣ Data Visualization
- Created visual plots to explore:
  - Tumor size distribution
  - Diagnosis result balance (Benign vs. Malignant)
  - Correlation heatmap for all features

### 3️⃣ Dataset Splitting
- Split data into:
  - **Training Set**: 70%
  - **Validation Set**: 15%
  - **Test Set**: 15%

### 4️⃣ Logistic Regression Implementation (from Scratch)
- Implemented `logistic_regression()` using:
  - Gradient descent
  - Cross-entropy loss
  - Optional bias term (`add_intercept`)
- Inputs:
  - `X`: Feature matrix
  - `Y`: Labels
  - `learning_rate`
  - `num_iterations`
  - `add_intercept`

### 5️⃣ Training & Evaluation
- Trained the model on the training set
- Evaluated using:
  - Validation and test accuracy
  - Performance comparison across different learning rates
- Visualized performance metrics during training

### 6️⃣ Bonus: Performance Metrics
- Calculated and explained:
  - **Precision**
  - **Recall**
  - **F1 Score**

---

## 🧪 Technologies Used

- **Python 3**
- **NumPy** – numerical operations and matrix math
- **Pandas** – data loading and preprocessing
- **Matplotlib / Seaborn** – visualizations
- *(No PyTorch, TensorFlow, or scikit-learn used)*

