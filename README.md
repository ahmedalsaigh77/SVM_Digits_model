# Handwritten Digit Classification using SVM and MLflow

## Overview

This project implements a machine learning system for handwritten digit classification using a Support Vector Machine (SVM) model.

The system receives an image of a handwritten digit, processes the image, and predicts the corresponding digit using a trained SVM classifier.

The project also integrates MLflow for experiment tracking, model management, and performance monitoring.

---

## Features

- Handwritten digit recognition.
- Image preprocessing and normalization.
- SVM classification model.
- Model saving and loading.
- Performance evaluation.
- MLflow experiment tracking.
- Logging of predictions and metrics.
- Web-based user interface for interaction.

---

## Dataset

The model is trained using the Scikit-learn Digits dataset.

Dataset characteristics:

- Number of samples: 1797
- Number of classes: 10
- Classes: digits from 0 to 9
- Image size: 8 × 8 pixels
- Features: 64 pixel values

---

## Machine Learning Pipeline

The workflow consists of the following steps:

1. Load the dataset.
2. Split data into training and testing sets.
3. Apply feature scaling using StandardScaler.
4. Train an SVM classifier.
5. Evaluate model performance.
6. Save the trained model.
7. Use the model for digit prediction.

---

## Model

Algorithm:

- Support Vector Machine (SVM)

Configuration:

- Kernel: RBF
- C: 1.0
- Gamma: Scale

---

## Evaluation Metrics

The model is evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report

The classification report includes:

- Precision
- Recall
- F1-score
- Support

---

## MLflow Tracking

MLflow is used to track:

- Model parameters.
- Evaluation metrics.
- Prediction results.
- Execution time.
- Generated artifacts.

Tracked information helps compare experiments and monitor model performance.

---

## Project Structure
DigitClassifier/

│
├── app.py
├── train.py
├── model.pkl
├── scaler.pkl
├── requirements.txt
│
├── templates/
│ └── index.html
│
├── static/
│ ├── style.css
│ └── script.js
│
├── uploads/
│
└── mlruns/

---

## Installation

Clone the repository:

```bash
git clone <repository-url>'''

## Install dependencies:
pip install -r requirements.txt

## Training model
python train.py

The training process will:

- Load the dataset.
- Train the SVM model.
- Evaluate the model.
- Save the trained model and preprocessing scaler.

---

## Running the System

Start the application:


python app.py


Then open the browser and access:


http://127.0.0.1:5000


---

## Technologies Used

- Python
- NumPy
- Scikit-learn
- OpenCV
- MLflow
- Joblib
- HTML
- CSS
- JavaScript

---

## Future Improvements

- Use larger handwritten digit datasets.
- Improve image preprocessing techniques.
- Train deep learning models.
- Compare multiple machine learning algorithms.
- Add more advanced experiment tracking.

---
