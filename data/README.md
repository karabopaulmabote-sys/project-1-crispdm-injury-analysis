# Dataset: Workplace Accident Records

**File:** `accidents.csv`  
**Source:** Publicly available dataset containing structured workplace incident reports.  
**Format:** CSV

## Description
The dataset contains individual incident records reported across different industries and provinces. Each row represents a single incident with details such as:

- Title of accident  
- Date  
- Province and city  
- Industry and sub-industry  
- Company name and ownership type  
- Accident type  
- Number of deaths  
- Number of injuries  
- Number of individuals punished  
- Financial penalties  

These attributes offer a structured view of workplace incidents, making the dataset suitable for exploratory analysis and supervised learning.

## Use in Project
This dataset is used for **Incident Severity Classification**, following the CRISP-DM framework. It supports the following tasks:

### 1. Data Understanding  
- Inspect structure, categories, and missingness  
- Explore incident types, industries, and locations  
- Understand injury and fatality patterns  

### 2. Data Preparation  
- Clean categorical fields  
- Standardise labels  
- Parse injury and fatality ranges  
- Engineer the severity target variable

### 3. Modelling  
Machine learning classifiers used include:  
- Decision Tree  
- Naïve Bayes  
- K-Nearest Neighbours (KNN)

### 4. Evaluation  
Models are assessed using accuracy, confusion matrices, and interpretability.

## Target Variable: Three-Class Severity
Severity is engineered into **three distinct classes** using fatalities and injuries:

### **Class 0 — Low Severity**  
- No deaths  
- 0–1 injuries  
- Minor impact, limited harm

### **Class 1 — Moderate Severity**  
- No deaths  
- 2–9 injuries  
- Noticeable harm, multiple affected individuals

### **Class 2 — High Severity**  
- At least one death  
- OR  
- 10+ injuries  
- Significant impact involving fatalities or high casualty counts

## Pre-processing Notes
Before modelling, the dataset is cleaned and prepared through:

- Handling missing or ambiguous values  
- Normalising industry, province, and ownership labels  
- Converting injury and fatality ranges into numerical or ordinal values  
- Constructing the three-class severity target  
- Selecting feature columns for training  

All processing steps are documented inside the notebook.

## Licensing
This dataset is used strictly for educational, academic, and non-commercial analysis.
