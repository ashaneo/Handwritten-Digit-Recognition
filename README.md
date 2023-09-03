# Handwritten Digit Recognition using SVM

A simple project for recognizing handwritten digits using Support Vector Machines (SVM).

## Overview

This project demonstrates the use of SVM for recognizing handwritten digits. It includes steps for capturing images of handwritten digits, preprocessing the images, training an SVM model, and evaluating its accuracy.

## Requirements

- Python 3.11
- Libraries:
  - `pyscreenshot` (for capturing screen images)
  - `opencv-python` (for image processing)
  - `joblib` (for model persistence)
  - `scikit-learn` (for SVM and evaluation)
  - `pandas` (for data handling)
  - `matplotlib` (for visualization)

You can install these requirements using pip:

```bash
pip install pyscreenshot opencv-python joblib scikit-learn pandas matplotlib

#Data Collection
Images of handwritten digits are captured from the screen using the pyscreenshot library. The images are then preprocessed, converted to grayscale, and resized to 28x28 pixels for compatibility with the model.

#Creating the Dataset
Captured images are saved in a CSV file (dataset.csv). Each row in the CSV file represents a digit image. The label (digit) and pixel values (0 or 1) for each pixel in the 28x28 grid are stored in the file.

#Model Training
A Support Vector Machine (SVM) classifier with a linear kernel is used for digit recognition. The dataset is split into training and testing sets. The model is trained on the training set and saved for later use.

#Model Evaluation
The accuracy of the trained model is calculated by comparing the predicted labels with the actual labels in the test set.

