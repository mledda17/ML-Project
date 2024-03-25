# Network Requests Classification Using Machine Learning

## Overview
This project tackles the challenge of identifying and classifying network traffic as either normal or malicious, based on a dataset taken from Kaggle. Our goal is to provide a robust model capable of distinguishing between benign and harmful network requests, contributing to enhanced cybersecurity measures.


## Problem Statement
With the growing number of cyber-attacks, it's crucial to develop systems capable of detecting malicious network traffic accurately. Our project utilizes machine learning techniques to classify network requests effectively, helping in the early detection of potential threats.


## Dataset
The dataset used in this project is sourced from the CSIC 2010 Web Application Attacks dataset on Kaggle. It includes 17 columns with samples labeled as "Normal" and "Anomalous", focusing mainly on the URL request and Payload features.


## Methodology
Our approach involves several key steps:

* **Data Pre-processing**: Initial data cleaning and preparation, including the handling of imbalanced data.
* **Feature Engineering**: Utilizing N-gram analysis to capture context and relationships within the data.
* **Model Selection and Cross-Validation**: Implementing a 6-fold cross-validation strategy and evaluating multiple classifiers, including SVM, Multinomial Logistic Regression, and Random Forest.
* **Hyper-Parameters Tuning**: Fine-tuning model parameters to achieve optimal performance.


## Results
The Random Forest classifier demonstrated the best performance, achieving an average accuracy of 98% ± 0.12, with optimal hyperparameters being n_estimators=200 and max_features='log2'.

## Installation and Usage
This project is available as a Colab notebook. To run it, simply follow these steps:

1. Open the python notebook present in this GitHub Repository
2. Save a copy of the notebook to your Google Drive.
3. Run the cells in sequence.

## Conclusions
While the classifiers have shown promising results on the dataset, it's important to note that achieving high accuracy does not guarantee generalization to all types of network traffic. Continuous evaluation and updating with new data are crucial for maintaining the model's effectiveness.
