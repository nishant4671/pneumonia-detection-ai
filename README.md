# Pneumonia Detection from Chest X-Rays using Deep Learning

## Project Overview
This project implements a Convolutional Neural Network (CNN) to classify chest X-ray images as Normal or Pneumonia.

## Results
- **Test Accuracy**: 79.5%
- **Precision (Pneumonia)**: 76%
- **Recall (Pneumonia)**: 99%
- **F1-Score (Pneumonia)**: 86%
- **Precision (Normal)**: 97%
- **Recall (Normal)**: 47%

## Model Architecture
The CNN model consists of:
- 4 Convolutional layers with ReLU activation
- MaxPooling layers for downsampling
- Dropout layer for regularization
- Dense layers for classification

## Files
- `Pneumonia_Detector.ipynb`: Complete implementation notebook
- `grad_cam_results.png`: Model interpretation visualizations

## Dataset
Source: Chest X-Ray Images (Pneumonia) on Kaggle
- Total Images: 5,863
- Training Set: 5,232 images (3,875 Pneumonia, 1,357 Normal)
- Test Set: 624 images (390 Pneumonia, 234 Normal)

## Ethical Considerations
This is NOT a medical device. It is a demo project and must never be used for real clinical diagnosis.
