# Lung_cancer_stages_detection_using_machine_learning
Machine Learning project using a hybrid model combining Xception and MobileNetV2 for lung cancer stage prediction. Trained on the IQ-OTH/NCCD CT scan dataset, the model classifies images into Normal, Benign, and Malignant (Stages 1–3). Streamlit is used for the front end. Image preprocessing and performance metrics like accuracy, precision, and F1-score are applied to ensure reliable results.
# Health Prediction Models Deployment

## Overview

This repository contains a hybrid deep learning model for predicting lung cancer stages—Normal, Benign, and Malignant. The model combines the strengths of Xception and MobileNetV2 architectures to enhance classification accuracy. The user interface is developed using Streamlit, providing an interactive and user-friendly platform for lung cancer stage prediction.

## Table of Contents

1. [Proposed Model](#proposed-model)
2. [Datasets](#datasets)
3. [Machine Learning Models](#machine-learning-models)
4. [Streamlit](#streamlit)
5. [Comparisions](#comparisions)


## Proposed Model

![image](https://github.com/user-attachments/assets/52cc9eff-360a-4a7b-bd9a-c0c8fd71c1c5)
The architecture illustrates a complete lung CT scan image classification system using a hybrid deep learning model combining Xception and MobileNetV2. The process starts with a user-friendly interface where users can register, log in, and upload CT scan images. Uploaded images undergo preprocessing such as normalization, resizing, and augmentation to prepare for analysis. The preprocessed image is passed to the hybrid model, where MobileNetV2 extracts fast, efficient features and Xception captures deeper patterns. The combined features are used to classify the image into Normal, Benign, or Malignant Stages 1–3. The results are interpreted, a report is generated, and it's delivered to the user via the interface and stored for future use.

## Datasets

The model uses the IQ-OTH/NCCD Lung Cancer CT Scan Dataset, a publicly available and widely used dataset for developing lung cancer detection systems. It contains high-quality CT scan images categorized into Normal, Benign, and Malignant stages. The dataset is well-organized with separate folders for each category.

## Machine Learning Models

The proposed model is implemented in the 'xception+mobilenetv2.py' file and is designed to classify lung cancer CT scan images into three categories: Normal, Benign, and Malignant. It is a hybrid model that leverages the strengths of two powerful deep learning architectures—Xception and MobileNetV2. Xception improves feature extraction by using depthwise separable convolutions, which enhances accuracy without significantly increasing computational cost. MobileNetV2, on the other hand, is optimized for speed and efficiency, making it ideal for lightweight applications. By combining these two models, the hybrid architecture achieves a balance between high performance and computational efficiency, making it well-suited for medical image classification tasks.

## Streamlit

The 'final.py' contains the Streamlit web application for deploying and interacting with the lung cancer prediction model. The application allows users to upload CT scan images and receive predictions for the corresponding lung cancer stage—Normal, Benign, or Malignant (Stages 1–3).

## Comparisions

| Models                         | Accuracy | Precision | Recall | F1 Score |
|-------------------------------|:--------:|:---------:|:------:|:--------:|
| Hybrid CNN (Xception + MobileNetV2) |   0.96   |   0.94    |  0.94  |   0.94   |
| Xception                      |   0.85   |   0.84    |  0.85  |   0.85   |
| MobileNetV2                   |   0.78   |   0.77    |  0.77  |   0.76   |
| ResNet50                      |   0.93   |   0.92    |  0.92  |   0.91   |



