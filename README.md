# Machine Vibration Classification

## Overview
This project focuses on classifying machine vibration data using various machine learning algorithms. The dataset consists of vibration signals from two different machines recorded at 10 million samples per second. The goal is to extract features from these signals and use them to accurately identify the machine type.

## Installation
To run this project, you'll need Python and the following libraries. You can install them using pip:

```bash
pip install numpy pandas scikit-learn pywt matplotlib tqdm
```

Usage
Download the vibration data files (S2_train_10msps_1sec.dat and S3_train_10msps_1sec.dat) and place them in a directory named Dataset.
Run the Jupyter Notebook or Python script to execute the classification pipeline.
The models used in this project include:
Support Vector Classifier (SVC)
k-Nearest Neighbors (KNN)
Decision Trees
Stacking Classifier
Data Preparation
The dataset is loaded from binary files and segmented into smaller chunks for feature extraction. Each segment contains a set of vibration data points.

Feature Extraction
Key features extracted from each segment include:

Mean
Variance
Skewness
Kurtosis
Dominant Frequency
Total Power
Wavelet Features (using Discrete Wavelet Transform)
Model Evaluation
Each model is evaluated using k-fold cross-validation. The evaluation metrics include accuracy, confusion matrix, precision, recall, and F1 score.

Results
The results show that the Support Vector Classifier with an RBF kernel achieved the best performance, with an accuracy of approximately 97%.
