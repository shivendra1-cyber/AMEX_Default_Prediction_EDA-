# American Express Credit Default Prediction Project
![Uploading image.png…]()


## Overview

Welcome to the American Express Credit Default Prediction Project repository. This project is aimed at developing a comprehensive credit risk prediction system for American Express, a leading financial services company. The project's primary objective is to leverage advanced machine learning techniques to optimize lending decisions, enhance the customer experience, and ensure the financial stability of the business.

## Data

### Data Source

The project utilizes a dataset containing information about American Express customers. This dataset includes a combination of numerical and categorical features that provide valuable insights into customer behavior and financial history.

### Data Preprocessing

To ensure the accuracy and effectiveness of our models, several critical data preprocessing steps have been undertaken:

- **Class Imbalance**: The training data reveals that 26% of American Express customers have defaulted on their credit. To address this imbalance, we employ the StratifiedKFold technique for cross-validation, ensuring that the model performs well across both default and non-default cases.

- **Handling Missing Data**: The dataset contains missing values, a common challenge in real-world datasets. While decision-tree-based algorithms can naturally handle missing values, neural networks, another component of our project, require imputation to ensure accurate predictions.

- **Time Series Modeling**: Approximately 80% of American Express customers have 13 statements, while the remaining 20% have 1 to 12 statements. We apply time series modeling to the 20% with fewer statements, and employ linear interpolation to fill in missing values. This process allows us to capture the temporal dimension of the data effectively.

- **Categorical Features**: The dataset includes eleven categorical features. Exploratory data analysis reveals distinct distributions for these features with respect to different target classes (0 and 1), indicating that they hold valuable information for predicting credit default.

## Model Building

The project encompasses various modeling approaches tailored to the specific challenges posed by credit risk prediction:

1. **Decision-Tree Models**:
   - Decision-tree models are a versatile tool in this project. They are used for handling class imbalance, managing missing values, and modeling the last statement for a subset of American Express customers. Importantly, decision trees can naturally accommodate missing values without requiring imputation.

2. **Neural Networks**:
   - Neural networks, known for their powerful predictive capabilities, are applied to credit default prediction. Due to their sensitivity to missing values, we diligently impute the missing data to ensure neural networks can be effectively utilized.

3. **Categorical Variable Modeling**:
   - In a separate notebook, we delve into the modeling of categorical variables. These variables are shown to contain valuable information related to the target variable, further enhancing the accuracy of our credit risk predictions.

## Key Findings

The analysis of the American Express credit default prediction project has yielded several key findings:

- The dataset reveals a significant default rate of 26%, highlighting the importance of robust risk management in lending decisions.

- Decision-tree models serve as a reliable and interpretable method for addressing class imbalance and effectively handling missing data, making them a valuable asset in credit risk prediction.

- Neural networks, while a potent tool in predictive modeling, require careful preprocessing and imputation of missing values to achieve optimal results in credit default prediction.

- Categorical features exhibit distinct distributions in relation to credit default, underscoring their significance in predicting default risk.

## Folder Structure

For your convenience, the project repository is organized as follows:

- `notebooks/`: This directory contains Jupyter notebooks with detailed code and explanations for various modeling tasks.

- `data/`: Here, you can access the dataset and other data-related resources used in the project.

- `results/`: This folder houses the model results and outputs, providing a reference for evaluating the performance of our credit default prediction models.

- `scripts/`: You can find utility scripts and code snippets for data preprocessing, manipulation, and other essential tasks in this directory.

Feel free to explore and utilize these resources to gain deeper insights into the American Express Credit Default Prediction Project.

We appreciate your interest in our project, and we hope that it provides valuable insights into credit risk prediction and management.

Please note that this README is subject to updates and revisions as the project progresses. Thank you for being a part of this journey!

