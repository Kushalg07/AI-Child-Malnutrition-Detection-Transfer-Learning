# 🧠 AI-Based Child Malnutrition Detection using Lightweight CNNs

Deep Learning framework for automated child nutritional status classification using **MobileNetV2** and **ShuffleNetV2** with transfer learning and Grad-CAM interpretability.

---

## 📌 Overview

Child malnutrition is a critical global health challenge, particularly in low-resource regions. Early detection plays a crucial role in timely medical intervention and improved health outcomes.

This project implements a deep learning-based image classification system to automatically categorize child images into:

- 🟢 **Nourished (Healthy)**
- 🔴 **Malnourished (Unhealthy)**

The system leverages lightweight convolutional neural networks optimized for deployment in mobile and resource-constrained environments.

---

## 🎯 Objectives

- Develop an automated malnutrition classification framework
- Compare MobileNetV2 and ShuffleNetV2 performance
- Analyze optimizer strategies (Adam vs SGD)
- Evaluate using comprehensive performance metrics
- Apply Grad-CAM for model interpretability

---

## 🏗️ Model Architectures

### 🔹 MobileNetV2
- Inverted residual blocks
- Depthwise separable convolutions
- Linear bottlenecks
- Efficient for mobile deployment

### 🔹 ShuffleNetV2
- Channel split and shuffle mechanism
- Low computational cost (FLOPs)
- Designed for edge devices

Both models are initialized with **ImageNet pretrained weights** and fine-tuned for binary classification.

---

## 📊 Experimental Results

### 🏆 Best Model Performance

| Model          | Optimizer | Epochs | Accuracy |
|---------------|------------|--------|----------|
| MobileNetV2   | SGD        | 50     | **97.97%** |
| ShuffleNetV2  | Adam       | 100    | 96.95% |

### 📈 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- ROC Curve
- Confusion Matrix

---

## 🔬 Model Interpretability

Grad-CAM visualization is applied to highlight the image regions influencing predictions.

This improves:
- Transparency
- Trust in medical AI systems
- Explainability for healthcare professionals

---

## 📂 Dataset Details

- Two classes: Nourished and Malnourished
- Training samples: 1657
- Validation samples: 503
- Image size: 224 × 224
- Normalization: ImageNet mean and standard deviation

⚠️ **Important:**  
The dataset used in this project was synthetically generated using Stable Diffusion.  
Future work includes validation using real-world pediatric datasets.

---

## ⚙️ Training Configuration

- Loss Function: Binary Cross Entropy
- Optimizers: Adam, SGD
- Learning Rate: 0.0001
- Batch Sizes: 24, 32, 40
- Epochs: 50–150
- Transfer Learning Enabled

---

## 📁 Project Structure
