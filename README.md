Assignment Week 6 - B. Miller
Overview

This repository contains my solutions for Week 6 Homework, which focuses on predictive modeling using two datasets:

BRCA dataset: Predicting tumor malignancy (y = M/B) using tumor features.

SBA dataset: Predicting loan approval (Loan_Status) using small business attributes.

The goal is to explore predictor variables, build classification models, apply transformations, and evaluate model performance using ROC curves and other metrics.

Contents

Assignment_Week6_BM.Rmd — R Markdown file containing all analyses, plots, and results.

Plots: Density plots, scatter plots, and histograms visualizing predictor-response relationships.

Models: Logistic regression, transformations (Box-Cox), and nonlinear term experiments.

Evaluation: ROC curves, AUC calculations, confusion matrices, and sensitivity/specificity analysis.

BRCA Dataset Analysis

Explored relationships between tumor features (radius, texture, perimeter, area) and malignancy.

Built logistic regression models to predict malignancy.

Evaluated model performance with ROC curves and calculated AUC (~0.7975 for baseline model).

Determined cutoff probabilities to achieve 90% true positive rate.

SBA Dataset Analysis

Checked for near-zero variance predictors and identified skewed distributions.

Applied Box-Cox transformation to quantitative predictors to normalize distributions.

Built logistic regression models using both original and transformed data.

Evaluated ROC curves and AUC for model improvement.

Tested nonlinear terms (squared predictors) to further improve model performance (small consistent improvements observed).

Key Packages

tidyverse — Data manipulation and visualization.

caret — Model training and evaluation.

dslabs — BRCA dataset.

pROC — ROC curves and AUC calculation.
