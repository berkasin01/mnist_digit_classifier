# MNIST Digit Classifier with Data Augmentation
Handwritten digit classification on the MNIST dataset using Random Forest, with a custom data augmentation pipeline to expand the training set.

## Dataset
70,000 images from the MNIST dataset, expanded to 210,000 with augmentation. Each image is 28x28 pixels flattened to 784 features.

## Augmentation
Custom augmentation pipeline built from scratch using torchvision and scipy. Each original image produces 2 rotated variants and 2 shifted variants.

-Random rotation (up to 10 degrees)
-Random pixel shifting

## Model
RandomForestClassifier with 100 estimators trained on StandardScaler normalised data.
Results

## Accuracy: 99%
Weighted average F1: 0.99
Consistent performance across all 10 digit classes

## Stack
Python, scikit-learn, torchvision, scipy, pandas, matplotlib
