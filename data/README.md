Dataset: Workplace Injury and Illness Claims

File: nz-injury-statistics-work-related-claims-2018-csv.csv

Source: Public dataset originally downloaded from Kaggle.

Format: CSV, multi-year panel data.

Description

The dataset contains annual counts of workplace injury and illness claims grouped by multiple demographic and industry attributes. Each row represents a combination of:

Year

Sex

Age group

Geographic region

Employment status

Occupation

Injury/Illness group

Type of injury/disease

Industry

Industry subgroup

Value (claim count)

Measure

Status

Use in Project

This dataset is used in Project 1 – CRISP-DM Data Science Lifecycle for the following tasks:

1. Data Understanding:
Exploration of categories, distributions, missingness, and relationships.

2. Data Preparation:
Cleaning, renaming, grouping, encoding, and fixing categorical structure.

3. Modelling (Simple Supervised Learning):
To align with the MEng coursework, a small modelling component is included:

Decision Tree

Naïve Bayes

K-Nearest Neighbours (KNN)

These models are used to predict a target variable such as injury type, injury group, or industry, depending on the final formulation.

4. Evaluation:
Performance assessed using accuracy, confusion matrices, and related metrics.

5. Insights:
Simple, interpretable explanations that connect back to the cleaned data.

Pre-processing

The dataset undergoes several preparation steps before modelling, including:

Standardising text labels

Removing empty categories

Encoding categorical features

Filtering out “Total” rows where needed

Validating the numerical field (Value)

These steps are documented inside the notebook.

Licensing

The dataset is used strictly for educational, academic, and non-commercial analysis under the terms of its original open data source.
