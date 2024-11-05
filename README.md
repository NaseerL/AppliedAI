# Midterm Exam - ECGR 8119: Applied AI

## Overview
This project involves a classification task using a Cat vs. Dog dataset sourced from Kaggle. The dataset was processed and trained using MobileNetV2, and results were compared between two models.

### Dataset Preparation
- **Dataset Source**: [Kaggle Cat vs. Dog Dataset](link_to_dataset)
- **Image Resizing**: All images were resized to 128x128 pixels.

## Model A
Model A utilizes the MobileNetV2 architecture to classify images in the dataset. Training results and performance metrics are documented in `ModelAvsModelB.ipynb`.

## SRGAN Implementation
A Super-Resolution Generative Adversarial Network (SRGAN) was developed based on the original SRGAN paper. The implementation details are as follows:
- **Generator Input**: 32x32 pixel images.
- **Generator Output**: Generates high-resolution 128x128 pixel images.
- **Discriminator**: Used to distinguish between original 128x128 images and the generated ones.
- **Training**: The model was trained for 150 epochs.
- **Future Improvements**: It is recommended to train the model for more epochs to achieve better results. Detailed results are shared in `SRGAN.ipynb`.

## Model B
Model B was developed using a modified dataset:
- **Subset Selection**: 2,500 images were selected from the original dataset.
- **Image Resizing**: These images were resized to 32x32 pixels and then processed through the generator to produce 128x128 images.
- **Dataset Integration**: The generated images were added back into the original dataset.
- **Training**: Model B was trained using the same approach as Model A.
- **Metrics**: The performance metrics include accuracy, F1 score, AUC, and loss. Results are documented alongside Model A.

## Conclusion
This project explores the application of MobileNetV2 for image classification, alongside the use of SRGAN for image enhancement. The comparative analysis of both models provides insights into their performance and effectiveness in classifying images.
