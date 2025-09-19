# Pneumonia Detection from Chest X-Rays using Deep Learning

## Project Overview
This project implements a Convolutional Neural Network (CNN) to classify chest X-ray images as Normal or Pneumonia. The goal is to demonstrate an end-to-end deep learning workflow for medical image analysis.

## Results
- **Test Accuracy**: 79.5%
- **Precision (Pneumonia)**: 76%
- **Recall (Pneumonia)**: 99%
- **F1-Score (Pneumonia)**: 86%
- **Precision (Normal)**: 97%
- **Recall (Normal)**: 47%

## Confusion Matrix
| | Predicted Normal | Predicted Pneumonia |
|---|---|---|
| **Actual Normal** | 109 | 125 |
| **Actual Pneumonia** | 3 | 387 |

## Model Architecture
The CNN model consists of:
- 4 Convolutional layers with ReLU activation
- MaxPooling layers for downsampling
- Dropout layer for regularization (50%)
- Dense layers for classification

## Dataset
Source: [Chest X-Ray Images (Pneumonia) on Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)
- **Total Images**: 5,863
- **Training Set**: 5,232 images (3,875 Pneumonia, 1,357 Normal)
- **Test Set**: 624 images (390 Pneumonia, 234 Normal)

## Key Insights
1. **High Sensitivity**: The model detects 99% of pneumonia cases (only 3 missed cases)
2. **Specificity Challenge**: Only 47% of normal cases correctly identified (high false positives)
3. **Clinical Relevance**: Grad-CAM visualizations show the model focuses on lung areas

## Ethical Considerations
This is NOT a medical device. It is a demo project and must never be used for real clinical diagnosis.

## Files
- `Pneumonia_Detector.ipynb`: Complete implementation notebook
- `grad_cam_results.png`: Model interpretation visualizations
