# Phase 1 Project: Aircraft Safety Analysis

## Overview

This project aims to identify the safest aircraft for a company looking to diversify its portfolio by entering the aviation industry. The analysis includes data preparation, exploratory data analysis, and modeling to determine the key variables that make an aircraft safe.

[PowerPoint Presentation](https://github.com/Pfuglo1/Aviation-Analysis/blob/main/Phase%201.pptx)

[Tableau](https://prod-uk-a.online.tableau.com/#/site/pfuglo1e73a362b7f/workbooks/1082302?:origin=card_share_link)

## Table of Contents

1. [Business Understanding](#business-understanding)
2. [Data Understanding](#data-understanding)
3. [Data Preparation](#data-preparation)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Conclusions](#conclusions)
8. [Future Work](#future-work)
9. [Usage](#usage)
10. [Dependencies](#dependencies)

## Business Understanding

### Project Prompt
Your company is expanding into new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating airplanes for commercial and private enterprises but do not know anything about the potential risks of aircraft. You are charged with determining which aircraft are the lowest risk for the company to start this new business endeavor. You must then translate your findings into actionable insights that the head of the new aviation division can use to help decide which airc...

### Goal
Find the variables that make an airplane the safest and provide business recommendations based on these findings.

![Alt text](https://github.com/Pfuglo1/Aviation-Analysis/blob/main/Images/Model.PNG)

## Data Understanding

### Dataset Overview
The dataset contains records of aircraft crashes between 1948 - 2022. The data from 1948 - 1982 is limited, so those data points are excluded to focus on the majority of the volume following 1982.

#### Important Data Columns
1. **Aircraft Make and Model**: Information about the specific make and model of the aircraft involved in each incident.
2. **Aircraft Damage**: The severity of the damage to the aircraft.
3. **Severity of Injuries**: A count for each incident on the number of uninjured, minor, serious, and fatal injuries.
4. **Engine Type**: The type of engine on the aircraft.
5. **Number of Engines**: The number of engines on an airplane. The mean is 1 but can range from 1 to 8.

## Data Preparation

### Step 1: Load and Explore Dataset
The first step involves loading the dataset and performing initial exploration to understand its structure and contents. This includes checking for missing values, data types, and basic statistical summaries.

### Step 2: Data Cleaning
Cleaning the data by handling missing values, removing duplicates, and correcting any inconsistencies.

### Step 3: Feature Engineering
Creating new features that might be useful for the analysis, such as aggregating injury severities into a single metric or categorizing aircraft models based on size and usage.

### Step 4: Data Transformation
Encoding categorical variables, normalizing or standardizing numerical features, and splitting the data into training and testing sets.

## Exploratory Data Analysis

### Univariate Analysis
Analyzing individual variables to understand their distributions and identifying any potential outliers or anomalies.

### Bivariate Analysis
Exploring relationships between pairs of variables to identify potential correlations or patterns.

### Multivariate Analysis
Using techniques like correlation matrices and pair plots to examine interactions between multiple variables simultaneously.

## Modeling

### Model Selection
Choosing appropriate machine learning models to predict aircraft safety. This may include logistic regression, decision trees, random forests, and gradient boosting machines.

### Hyperparameter Tuning
Optimizing model performance by tuning hyperparameters using techniques like grid search or random search.

### Training and Validation
Training the models on the training dataset and validating their performance on the validation dataset.

## Evaluation

### Performance Metrics
Evaluating models using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.

### Model Comparison
Comparing the performance of different models to select the best one for predicting aircraft safety.



## Usage

### Running the Notebook
To run the Jupyter Notebook and reproduce the analysis:

1. Clone the repository:
    ```bash
    git clone https://github.com/Pfuglo1/Aviation-Analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd Aviation-Analysis
    ```
3. Install the required dependencies (see below).
4. Open the Jupyter Notebook:
    ```bash
    jupyter notebook phase_1_project.ipynb
    ```

### Dependencies
To install the required packages, use the following command:
```bash
pip install -r requirements.txt


The requirements.txt file should include all necessary libraries such as:

pandas
numpy
scikit-learn
matplotlib
seaborn