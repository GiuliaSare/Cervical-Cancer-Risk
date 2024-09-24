# Cervical Cancer Risk: A Case Study

**Authors**: Giulia Saresini, Nicola Perani, Sara Nava  
**University**: University of Milano-Bicocca – Master's Degree in Data Science

## Overview
This project aims to develop a predictive model to identify high-risk cervical cancer cases requiring biopsy using a Kaggle dataset with 36 variables. The study addresses data imbalance and evaluates model performance, highlighting the J48 algorithm's robustness and high recall. Future work will focus on ensemble methods and model fine-tuning.

## Table of Contents
- [Introduction](#introduction)
- [Pre-processing](#pre-processing)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Test Results](#test-results)
- [Conclusions](#conclusions)
- [References](#references)

## Introduction
Cervical cancer remains a global health issue, with 11,000 new cases annually in the U.S. This project investigates risk factors to identify cases needing biopsy, using data from Kaggle and the UCI Repository.

## Pre-processing
- **Categorical Variables**: Converted and encoded to eliminate decimal places.
- **Missing Data**: Excluded attributes with >30% missing data; imputed others with median/mode.
- **Class Imbalance**: Addressed using SMOTE for oversampling.
- **Dataset Partitioning**: 80% training, 20% testing.

## Model Training
Six classification models were trained: J48, Random Forest, Logistic Regression, Multilayer Perceptron (MLP), Naive Bayes, and SVM. Feature selection and data scaling were applied as needed.

## Model Evaluation
Models were evaluated using 10-fold cross-validation, with assessments on accuracy, sensitivity, specificity, and ROC curves.

## Test Results

### Balanced Data
| Model         | Accuracy | Recall |
|---------------|----------|--------|
| J48           | 0.947    | 0.818  |
| Random Forest | 0.940    | 0.545  |
| Logistic      | 0.954    | 0.818  |

### Imbalanced Data
| Model         | Accuracy | Recall |
|---------------|----------|--------|
| J48           | 0.940    | 0.818  |
| Random Forest | 0.934    | 0.818  |
| Logistic      | 0.934    | 0.818  |

## Conclusions
The J48 model showed high recall and robustness. Future efforts will focus on ensemble methods and fine-tuning to improve cervical cancer risk assessment.
