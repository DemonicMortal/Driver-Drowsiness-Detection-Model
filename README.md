# Attention-Guided Driver Drowsiness Detection

A deep learning based video driver drowsiness detection system built using an Attention-Guided CNN-Transformer architecture. The system processes sequential video frames to detect driver fatigue and drowsiness using temporal video understanding.

## Overview

This project focuses on detecting driver drowsiness from video sequences using a hybrid deep learning pipeline:

* MobileNet-based CNN for spatial feature extraction
* Attention mechanism for important frame weighting
* Transformer encoder for temporal sequence modeling
* OpenCV for video processing and real-time monitoring
* PyTorch for model development and training

The model is trained on the SUST Driver Drowsiness Dataset and designed for future real-time deployment.

---

# Features

* Video-based driver drowsiness detection
* Attention-Guided CNN-Transformer architecture
* Temporal sequence learning using Transformer Encoder
* Frame extraction and preprocessing pipeline
* Early stopping and checkpoint saving
* Evaluation metrics and confusion matrix
* Real-time webcam monitoring support
* Cached frame pipeline for faster training

---

# Tech Stack

* Python
* PyTorch
* OpenCV
* NumPy
* scikit-learn
* torchvision
* Matplotlib

---

# Model Architecture

```text
Video Input
     ↓
Frame Extraction
     ↓
MobileNet CNN
     ↓
Attention Module
     ↓
Transformer Encoder
     ↓
Temporal Attention Pooling
     ↓
Classifier
     ↓
Drowsy / Not Drowsy
```

---

# Dataset

Dataset Used:

* SUST Driver Drowsiness Dataset (SUST-DDD)

The dataset contains video samples categorized into:

* Drowsiness
* Not Drowsiness

---

# Training Details

* Loss Function: CrossEntropyLoss
* Optimizer: Adam
* Learning Rate Scheduler: StepLR
* Early Stopping Enabled
* Attention-Based Temporal Pooling
* Validation Accuracy Achieved: ~83%

---

# Evaluation Metrics

The model was evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

# Real-Time Monitoring

The project also includes a real-time webcam monitoring pipeline using OpenCV.

Capabilities:

* Webcam frame capture
* Sequential frame buffering
* Real-time inference
* Drowsiness prediction display

---

# Future Improvements

* Face and eye-region detection
* Audio alert system integration
* Smartwatch physiological signal integration
* Web deployment using Streamlit or Flask
* Edge deployment on embedded systems

---

# Results

* Achieved approximately 83% validation accuracy
* Improved temporal learning using attention-guided transformer architecture
* Faster training achieved through cached frame preprocessing

---

# Author

Developed as part of an 8th Semester B.Tech CSE Major Project.
