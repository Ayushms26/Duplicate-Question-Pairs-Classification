
# Duplicate Question Pairs Classification

## Overview

This project implements a machine learning classifier to detect duplicate question pairs from a dataset of questions. The goal is to determine if two given questions are asking the same thing (binary classification: 1 for duplicate, 0 for non-duplicate). The project employs advanced text preprocessing techniques, feature engineering, and models such as Artificial Neural Networks (ANN), Support Vector Machines (SVM), and XGBoost.

The dataset consists of pairs of questions, and the classifier is trained to predict if a pair is duplicate. The performance of the model is evaluated using metrics like ROC AUC and F1 score.

## Dataset

The dataset used for this project contains pairs of questions from the Quora Question Pairs dataset. Each entry has the following columns:

- **question1**: The first question in the pair
- **question2**: The second question in the pair
- **is_duplicate**: Target variable indicating whether the pair of questions are duplicates (1) or not (0)

## Features

- **Text Preprocessing**: Includes techniques such as tokenization, stemming, stopword removal, and lemmatization.
- **Feature Engineering**: Used Word2Vec embeddings for generating vector representations of the questions.
- **Model Training**: Trains machine learning models including ANN, SVM, and XGBoost for classification.
- **Model Evaluation**: Models are evaluated using ROC AUC and F1 scores.

## Usage

- Run the main Python script or Jupyter Notebook to perform duplicate question pair classification.
- The script performs the following:
  - Loads and preprocesses the dataset
  - Generates features using Word2Vec embeddings
  - Trains and evaluates machine learning models (ANN, SVM, XGBoost)
  - Outputs performance metrics such as ROC AUC and F1 score

## Results

- **ANN** achieved the best performance with a robust **ROC AUC score of 0.87** and an **F1 score of 0.72**.
- The model was trained on 100,000 question pairs and achieved a training accuracy of **0.87** and a validation accuracy of **0.80**.

## Conclusion

This project demonstrates how machine learning algorithms can be used to detect duplicate question pairs effectively. The best-performing model (ANN) achieved strong results, with high accuracy and AUC scores, making it a useful tool for applications such as question answering systems.
