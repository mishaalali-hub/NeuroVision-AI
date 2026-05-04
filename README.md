# NeuroVision-AI

A Deep Learning project focused on brain tumor classification from MRI images using Convolutional Neural Networks (CNN) and Transfer Learning techniques.

This project applies modern computer vision methods to automatically classify brain MRI scans into multiple categories, demonstrating the real-world application of AI in medical imaging.

---

# Project Overview

The goal of this project is to build an intelligent image classification system capable of identifying different types of brain tumors from MRI scans.

The model performs **multi-class classification** into:

- Glioma
- Meningioma
- Pituitary Tumor
- Healthy

A transfer learning approach using a pre-trained CNN model is applied to improve performance and reduce training complexity.

---

# Dataset

- Brain MRI image dataset (multi-class)
- Organized into class-based directories
- Each folder represents a tumor type or healthy class
- Automatically labeled using directory structure

---

# Technologies Used

## Programming Language
- Python

## Libraries & Frameworks
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn

---

# Project Structure

```bash
NeuroVision-AI/
│
├── NeuroVision_Model.ipynb
├── dataset/ (MRI images - not uploaded due to size)
├── README.md
```

---

# Features Implemented

## 1. Data Preprocessing

- Directory-based dataset loading
- Automatic label extraction
- Train / Validation / Test split
- Image resizing
- Pixel normalization (0–255 → 0–1)

---

## 2. Data Augmentation

- Improves generalization
- Prevents overfitting
- Enhances dataset variability

---

## 3. CNN + Transfer Learning

- Pre-trained **MobileNetV2** used as feature extractor
- Base model weights frozen
- Custom classification head added

---

## 4. Model Architecture

The model includes:

- MobileNetV2 backbone (pre-trained)
- Global Average Pooling
- Dropout (regularization)
- Dense output layer (Softmax activation)

---

## 5. Training & Optimization

- Loss Function: Categorical Cross-Entropy
- Optimizer: Adam
- Regularization: Dropout + L2
- Backpropagation used for weight updates

---

## 6. Evaluation Metrics

- Accuracy
- Loss
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

# Algorithms Used

## 1. Convolutional Neural Networks (CNN)

### Why Used
- Best model for image classification
- Automatically learns spatial features
- High performance in computer vision tasks

### How It Works
- Extracts features using convolution layers
- Reduces dimensions using pooling
- Classifies images using dense layers

---

## 2. Transfer Learning (MobileNetV2)

### Why Used
- Reduces training time
- Improves accuracy with limited data
- Uses knowledge from large-scale datasets (ImageNet)

### How It Works
- Pre-trained model used as feature extractor
- Only final layers are trained
- Prevents overfitting and improves generalization

---

## 3. Backpropagation

- Computes gradients of loss function
- Updates model weights
- Improves prediction accuracy over time

---

# Model Performance

- Achieved strong classification performance on test data
- High accuracy and stable loss behavior
- Good generalization with minimal overfitting

Key observations:

- Healthy class achieved highest performance
- Some confusion between similar tumor types
- Model effectively learned visual patterns in MRI scans

---

# Results

The project successfully:

- Built a CNN-based medical image classifier
- Applied transfer learning effectively
- Achieved strong performance on unseen data
- Visualized training performance and predictions
- Demonstrated real-world AI application in healthcare

---

# Notebook Description

## NeuroVision_Model.ipynb

This notebook includes:

- Data loading and preprocessing
- Model building using MobileNetV2
- Training and validation
- Performance evaluation
- Confusion matrix and classification report
- Visualization of predictions

---

# Applications

- Medical image analysis
- Clinical decision support systems
- Automated tumor detection
- Healthcare AI solutions

---

# Academic Purpose

This project was developed for:

- Deep Learning coursework
- Computer Vision practice
- Understanding CNN and Transfer Learning
- Medical AI application development

---

# Future Improvements

- Use larger and more diverse datasets
- Fine-tune the pre-trained backbone
- Apply advanced architectures (ResNet, EfficientNet)
- Deploy as a web or mobile application
- Integrate explainable AI (Grad-CAM)

# License

This project is intended for academic and educational purposes only.
