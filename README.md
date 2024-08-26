# Fraud-Detection-Auto-Claims
Analyzed auto claims dataset to detect fraud using logistic regression and tested the hypothesis that claims above $10k are fraudulent.

## Project Overview

This project aims to predict fraudulent auto insurance claims to help reduce losses due to fraud. The dataset used consists of 975 records with 38 features, representing approved claims for auto repairs after accidents.

### Business Problem

The Fraud Claims Department at an auto insurance company faces challenges with identifying fraudulent claims due to the increase in online and mobile claims submissions. With limited time for claim processors to investigate, fraud detection is critical to prevent financial losses.

The company has lost millions due to fraud, making it a significant pain point. The goal of this project is to leverage data science to predict fraud and suspicious activity effectively.

### Hypothesis

The business sponsor hypothesized that auto insurance claims for repairs exceeding $10K might be fraudulent. The objective was to test this hypothesis and improve fraud detection mechanisms.

## Dataset Description

The dataset is a CSV file with 975 rows and 38 columns, each row representing a single person's claim data. Each claim has already been approved by the company. Features include various details about the claim, driver, and vehicle.

### Data Details

- **Number of Rows:** 975
- **Number of Columns:** 38
- **Features Include:** Claim amount, driver record, vehicle details, etc.

## Methodology

### Data Preparation

Data cleaning and preprocessing steps included handling missing values, encoding categorical variables, and feature scaling.

### Handling Class Imbalance

The dataset was imbalanced, with significantly fewer fraudulent claims compared to legitimate claims. To address this, under-sampling was performed on the legitimate claims to balance the dataset with the 406 fraudulent samples. This technique ensured that the model was not biased towards the majority class and improved the effectiveness of fraud detection.

### Model Selection

Logistic regression was chosen to predict the probability of a claim being fraudulent. This choice was based on its effectiveness for binary classification problems.


### Analysis

A scatter plot was created to visualize claims exceeding $10K and their fraud status. The analysis revealed that while many high-value claims are fraudulent, some are not, and fraud also occurs in claims below $10K.

## Insights and Results

The hypothesis that claims over $10K are more likely to be fraudulent was supported; however, the analysis uncovered additional insights:

- **Fraudulent Claims:** Claims over $10K often indicate fraud, but not all such claims are fraudulent.
- **Claims Under $10K:** Some fraudulent claims occur below the $10K threshold.

## Model Performance

The logistic regression model was evaluated on both training and testing data, showing strong performance:

- **Accuracy on Training Data:** 98.46%
- **Accuracy on Testing Data:** 98.77%

The high accuracy on both datasets indicates that the model generalizes well and is effective in predicting fraudulent claims.


Visualizations and performance metrics are included in the `/visualizations` folder.
