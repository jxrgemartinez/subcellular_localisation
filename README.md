# Protein Subcellular Localisation Prediction using Deep Learning

## Overview

This project, developed as part of academic cursus of the MSc in Bioinformatics, explores the application of various deep learning architectures to predict protein subcellular localization using Position-Specific Scoring Matrix (PSSM) data. The project is implemented in a Jupyter Notebook, showcasing different neural network models and techniques to improve prediction accuracy.

## Objective

The main objective of this project is to develop and compare different deep learning models for predicting protein subcellular localization. By utilizing PSSM data and experimenting with various architectures and techniques, we aim to identify the most effective approach for this prediction task.

## Features

The project implements and compares the following deep learning architectures:

1. Deep Neural Network (DNN)
2. Convolutional Neural Network (CNN)
3. CNN with Functional API
4. Residual Network (ResNet)

To improve model performance and address potential challenges, the following techniques are applied:

1. Class Weighting: To handle imbalanced datasets and improve prediction accuracy for underrepresented classes.
2. Data Augmentation: To increase the diversity of the training data and enhance model generalization.

## Results

The following table summarizes the accuracy results for each model under different conditions:

| Model   | Base   | Class Weights (CW) | Data Augmentation (Aug) |
|---------|--------|--------------------|-----------------------|
| CNN     | 82.05% | 82.20%             | 82.36%                |
| CNN_API | 79.06% | 80.63%             | 82.05%                |
| DNN     | 72.13% | 74.33%             | 74.33%                |
| ResNet  | 74.02% | 71.18%             | 72.28%                |

This table shows the performance of different models (CNN, CNN with Functional API, DNN, and ResNet) under three conditions:
- Base: The model's performance without any additional techniques
- CW: The model's performance with class weighting applied
- Aug: The model's performance with data augmentation

Key observations:
1. The CNN model consistently performs best across all conditions.
2. Class weighting and data augmentation generally improve model performance, with some exceptions.
3. The CNN_API model shows the most significant improvement with data augmentation.
4. Interestingly, the ResNet model's performance decreased with class weighting and only slightly improved with data augmentation.

## References
Almagro Armenteros, J. J., Sønderby, C. K., Sønderby, S. K., Nielsen, H., & Winther, O. (2017). DeepLoc: prediction of protein subcellular localization using deep learning. Bioinformatics (Oxford, England), 33(21), 3387–3395. https://doi.org/10.1093/bioinformatics/btx431