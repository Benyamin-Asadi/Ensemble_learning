# Machine Learning Ensemble Models Project

## Overview

This project implements and evaluates several ensemble machine learning models, including Bagging, Random Forest, AdaBoost, and Stacked Learners, for a classification task.
The goal is to train and optimize decision tree-based models to achieve high accuracy while preventing overfitting. The project includes hyperparameter tuning, performance evaluation on training and test datasets, and the use of K-Fold Cross-Validation to ensure robust model performance. 
The models are compared based on metrics such as accuracy, precision, recall, and F1-score, with a focus on finding the optimal number of estimators and hyperparameters for each approach.

## Features


- Bagging Implementation:





- Trains decision trees with limited depth to create a bagging classifier.



- Optimizes hyperparameters such as max_depth, min_samples_split, and min_samples_leaf using a grid search.



- Evaluates performance by varying the number of estimators to find the optimal configuration.



- Achieves a test accuracy of 0.8618, with precision, recall, and F1-score of approximately 0.8627, 0.8590, and 0.8608, respectively.



- Random Forest Model:





- Implements a Random Forest classifier, training multiple decision trees and evaluating performance.



- Achieves consistent performance across multiple runs, demonstrating robustness compared to single decision trees.



- Reports a test accuracy of 0.8528, with slight improvements in handling specific data patterns compared to the custom model.



- AdaBoost Implementation:





- Utilizes AdaBoost with a weak classifier to boost performance.



- Determines the optimal number of estimators for the AdaBoost model, achieving competitive results.



- Stacked Learners:





- Builds a meta-model by stacking multiple base models, including Random Forest, Gradient Boosting, and Decision Trees.



- Uses hyperparameter tuning to optimize base models, with best parameters reported (e.g., Random Forest: n_estimators=100, Gradient Boosting: learning_rate=0.1, max_depth=5, n_estimators=50).



- Achieves a test accuracy of 0.8718 for the meta-model, with precision, recall, and F1-score of 0.8602, 0.8864, and 0.8731, respectively.



- Overfitting Prevention:





- Employs K-Fold Cross-Validation to generate meta-features and prevent overfitting in the stacking process.



- Applies regularization techniques to control model complexity and improve generalization.



- Performance Metrics:





- Comprehensive evaluation of models using accuracy, precision, recall, and F1-score on both training and test datasets.



- Visualizes performance trends, such as accuracy versus the number of estimators, to guide model selection.
