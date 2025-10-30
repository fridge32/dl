# CNN Flower Classifier using TensorFlow

## Problem Statement
The objective of this project is to build a **Convolutional Neural Network (CNN)** model that can accurately classify images of flowers into multiple categories using the **TensorFlow Flowers dataset**.

## 📊 Dataset Used
- **Dataset:** `tf_flowers` (from TensorFlow Datasets)
- **Classes:** 5 flower categories
- The dataset is automatically downloaded when running the notebook.

## Model Architecture
The CNN architecture used:
- `Conv2D(32, 3x3)` + ReLU + MaxPooling
- `Conv2D(64, 3x3)` + ReLU + MaxPooling
- `Conv2D(128, 3x3)` + ReLU + MaxPooling
- Flatten → Dense(128, ReLU) → Dropout(0.5)
- Output: Dense(5, softmax)

**Optimizer:** Adam  
**Loss Function:** Sparse Categorical Crossentropy  
**Metrics:** Accuracy  
