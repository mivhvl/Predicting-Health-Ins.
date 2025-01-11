# README.md

## Project Overview
This project is focused on predicting whether a customer has health insurance based on a variety of demographic and economic factors. The goal is to identify uninsured customers so that companies can better target their resources and design personalized marketing strategies to encourage insurance adoption. By understanding the key factors that influence health insurance coverage, the company can also gain insights to address gaps in service delivery.

This project was part of a Kaggle competition, where it achieved 5th place.

## Motivation
The need to identify customers who do not have health insurance is critical for businesses looking to expand their customer base and tailor their services. By predicting uninsured customers, companies can take proactive measures to offer insurance and design targeted strategies that improve overall coverage rates. The analysis of demographic and economic factors helps to uncover patterns that influence insurance adoption, which can guide future decisions and strategies.

## Methodology
- **Data Collection:** The dataset includes various customer properties such as customer ID, sex, employment status, income, marital status, housing type, number of vehicles, age, state, gas usage, number of rooms, and recent move.
- **Data Preprocessing** 
- **Feature Selection:** Various feature selection techniques were used to identify the most important factors influencing health insurance coverage.
- **Modeling:** Multiple machine learning models were built and evaluated, including:
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Decision Trees
  - Random Forest
  - Support Vector Machines (SVM)
  - Neural Networks
  - XGBoost
- **Hyperparameter Tuning:** GridSearchCV was used to find the best hyperparameters for each model based on the F1 score.
- **Model Evaluation:** The models were evaluated using accuracy, precision, recall, and F1 score, with a focus on balancing performance across the classes (insured vs. uninsured).

## Results
- **Best Performing Models:** The Random Forest, Neural Networks, and XGBoost models provided the best performance for the given dataset, particularly after preprocessing with SMOTE.
- **Data Imbalance:** The dataset was imbalanced, with more insured customers than uninsured. SMOTE was applied to balance the data and improve the performance of the models, especially for the minority class.
- **Feature Importance:** Random Forest was used for feature selection, and it helped to improve the performance of other models like SVM.
- **Voting Classifier:** A voting classifier combining multiple models was also tested, yielding the best results (XGB, XGB without age ranges, SVM using only 15 most important features).

## Kaggle Competition
- **Rank:** 5th place in the Kaggle competition.
- **Objective:** Predicting uninsured customers using a variety of machine learning models and techniques to handle imbalanced datasets.

## Usage
1. Clone the repository:
   ```bash
   git clone <https://github.com/mivhvl/Predicting-Health-Ins..git>
   ```
2. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook

## Structure
- `dataset/`: Datasets
- `IDC.ipynb`: Analysis notebook

## License
Licensed under the MIT License.
