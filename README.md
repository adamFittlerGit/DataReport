# COMP4702: Machine Learning Project

## Overview

This project explores the efficacy of various machine learning models applied to a dataset containing traits of *Drosophila melanogaster* (fruit flies). Three models were analyzed in terms of classification and regression tasks:
- **Decision Trees**
- **Extreme Gradient Boosting (XGBoost)**
- **Multilayer Perceptron (MLP)**

The primary objectives were to classify the sex of the flies and predict their wing loading characteristics. Each model was tuned for optimal performance and evaluated based on accuracy, mean squared error (MSE), R² scores, and classification metrics.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Exploration and Preprocessing](#data-exploration-and-preprocessing)
3. [Model Implementations](#model-implementations)
   - Decision Trees
   - XGBoost
   - Multilayer Perceptron (MLP)
4. [Model Analysis](#model-analysis)
5. [Discussion](#discussion)
6. [Conclusion](#conclusion)

## Introduction

This study utilizes machine learning techniques to analyze traits from *Drosophila melanogaster*, widely used in genetics and developmental biology. Machine learning offers insights by handling complex datasets, especially in tasks like trait classification and prediction, which is integral to genetic research. This report investigates how well machine learning models can classify and predict traits based on physical and genetic data.

## Data Exploration and Preprocessing

1. **Visualization**: Initial analysis revealed patterns and distribution trends across features.
2. **Cleaning**: Removed redundant columns and handled missing values.
3. **Encoding**: Converted categorical variables into numerical formats.
4. **Normalization**: Standardized numerical features to ensure uniform scale across the dataset.
5. **Splitting**: Split data into training and test sets with stratification to maintain class balance.

## Model Implementations

### Decision Trees

- **Classifier**: Implemented using `DecisionTreeClassifier` from scikit-learn, tuned with grid search and cross-validation.
- **Regressor**: Utilized `DecisionTreeRegressor` with grid search and cross-validation, achieving high interpretability.

### Extreme Gradient Boosting (XGBoost)

- **Classifier and Regressor**: XGBoost models were optimized using Bayesian Search for hyperparameter tuning, ensuring computational efficiency. Implemented through scikit-learn’s pipeline to encapsulate preprocessing and model training.

### Multilayer Perceptron (MLP)

- **Architecture**: Built using PyTorch with a fully connected architecture to handle 17 input features.
- **Training Procedure**: Employed Adam optimizer and learning rate scheduling, with dropout and batch normalization to prevent overfitting.

## Model Analysis

- **Decision Trees**: Provided a solid baseline with high accuracy for classification tasks.
- **XGBoost**: Outperformed other models, especially in regression, demonstrating superior generalization ability.
- **MLP**: Flexibly captured complex nonlinear relationships but lagged behind XGBoost in regression accuracy.

## Discussion

Each model had its own advantages:
- **Decision Trees**: Simple, interpretable, and quick to train, making them suitable for datasets requiring minimal computational resources.
- **XGBoost**: High accuracy and low variance, ideal for complex prediction tasks.
- **MLP**: Capable of modeling intricate relationships but requires more computational resources and careful tuning.

## Conclusion

The XGBoost model was the best performer across tasks, achieving high accuracy, low bias, and low variance. Decision Trees provided a reliable baseline, and the MLP demonstrated the potential of neural networks for biological data analysis. The results of this study support further exploration of ensemble and deep learning methods in biological research.

## Resources

- Notebooks: [GitHub Repository](https://github.com/adamFittlerGit/DataReport)

---

*Author*: Adam Fittler  
*Course*: COMP4702 Machine Learning  
