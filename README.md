🧠 Applied Machine Learning Projects

This repository contains projects and assignments completed for my Applied Machine Learning class. Each project involves exploring machine learning models on real-world datasets, including model selection, training, evaluation, and interpretation.

📁 Project 1: Heart Disease Classification

Goal:
Predict the presence of heart disease in patients using classification models applied to the UCI Heart Disease Dataset
.

🧪 Models Implemented

Bernoulli Naive Bayes

Gaussian Naive Bayes

Linear Regression (used as a classifier)
📊 Dataset

Source: UCI Machine Learning Repository

Features: 13 clinical attributes including age, sex, cholesterol levels, resting blood pressure, etc.

Target: Presence (1) or absence (0) of heart disease

⚙️ Methods & Workflow

Preprocessing:

Handling missing values

Capping and binning

Binarizing features for BernoulliNB

One hot encoding and Standardization for GaussianNB and Linear Regression

Model training and evaluation using:

Accuracy

Confusion matrix

ROC/AUC curves

Discussion on the comparative performance of each model

📁 Files

heart_disease_classification.ipynb — Main notebook containing code, plots, and analysis.
heart_disease_classification_report.pdf - Analytical insights and findings report
README.md — This file.
