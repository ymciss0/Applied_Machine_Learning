# 🧠 Applied Machine Learning Projects

This repository contains projects and assignments completed for my Applied Machine Learning class. Each project involves exploring machine learning models on real-world datasets, including model selection, training, evaluation, and interpretation.

## 📁 Project 1: Heart Disease Classification

Goal:
Predict the presence of heart disease in patients using classification models applied to the UCI Heart Disease Dataset.

### 🧪 Models Implemented

Bernoulli Naive Bayes
Gaussian Naive Bayes
Linear Regression (used as a classifier)

### 📊 Dataset

Source: UCI Machine Learning Repository
Size: 303 observations × 14 features
Features: 13 clinical attributes including age, sex, cholesterol levels, resting blood pressure, etc.
Target: Presence (1) or absence (0) of heart disease
Class Imbalance: ~46% positive class

### ⚙️ Methods & Workflow

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

### 📁 Files

heart_disease_classification_final.ipynb — Main notebook containing code, plots, and analysis.
heart_disease_classification_report_final.pdf - Analytical insights and findings report

## 📁 Project 2: Bank Marketing Campaign Classification

Goal: Predict whether a bank client will subscribe to a term deposit using ensemble methods and boosting techniques applied to the UCI Bank Marketing Dataset.

### 🧪 Models Implemented

Decision Tree (baseline)
Random Forest
Gradient Boosting Machine (GBM)
XGBoost

### 📊 Dataset

Source: UCI Machine Learning Repository - Bank Marketing Dataset
Size: 41,188 observations × 20 features
Features: Client demographics, campaign details, and economic indicators
Target: Binary - client subscribed to term deposit (yes/no)
Class Imbalance: 11.3% positive class

### ⚙️ Methods & Workflow
Preprocessing:

Train-test split (80-20) with stratification before transformations to prevent data leakage
One-hot encoding for categorical variables
Standardization for continuous variables

Model training and evaluation using:

GridSearchCV with 5-fold cross-validation
Primary metric: F1-score (optimal for imbalanced data)
Secondary metrics: AUCPR, Accuracy
Confusion matrices and Precision-Recall curves
Feature importance analysis
Discussion on the comparative performance of each model

### 📁 Files

term_deposit_subscription_prediction.ipynb — Main notebook containing code, plots, and analysis
term_deposit_subscription_prediction.pdf — Analytical insights and findings report

## 📁 Project 3: Tiny Transformer for Next Token Prediction
Goal: Build and systematically evaluate a tiny transformer model for next token prediction on Shakespeare text, analyzing the impact of key hyperparameters on model performance.

### 🧪 Model Variations Implemented
Baseline (v1): 60 epochs, standard parameters
Experimental variations: Learning rate (v2), Batch size (v3), Sequence length (v4), Vocabulary size (v5), FFN dimension (v6), Embedding dimension (v7)

### 📊 Dataset
Source: Tiny Shakespeare (Karpathy's char-rnn repository)
Size: 581,009 tokens after Byte-Level BPE tokenization
Split: 80-20 train-test (464,787 train / 116,197 test sequences)
Sequences: 580,985 overlapping sequences of length 50 (baseline)

### ⚙️ Methods & Workflow
Architecture:

2 transformer blocks with single-head self-attention and causal masking
RMSNorm layers, learnable positional encodings, residual connections
Total parameters: 493,940

Training:

GridSearchCV-style hyperparameter exploration across 7 model versions \n
Primary metric: Perplexity (lower is better) \n
Secondary metrics: Accuracy, Loss \n
Validation curves and attention matrix visualization \n
Hardware: Tesla T4 GPU (~13 min average training time) \n

### 📁 Files

next_token_prediction.ipynb — Main notebook containing code, plots, and analysis
next_token_prediction.pdf — Analytical insights and findings report

README.md — This file.
