# Incident Severity Classification with CRISP-DM and Machine Learning
This project applies the full Data Science Lifecycle using the CRISP-DM framework. The dataset contains detailed records of workplace incidents across industries, provinces, and company types, including the number of injuries and fatalities associated with each incident. The goal is to classify incident severity using simple machine learning models and a structured workflow.

## Objectives
- Understand the structure and behaviour of the incident dataset  
- Clean and prepare the data for analysis  
- Create a clear severity target variable  
- Explore patterns across industries, incident types, ownership groups, and locations  
- Train simple machine learning models (Decision Tree, Naïve Bayes, KNN)  
- Evaluate model performance using standard metrics  
- Interpret the results in a practical and understandable way  

## CRISP-DM Workflow
**1. Business Understanding**  
Frame the problem and identify incident characteristics that relate to severity.

**2. Data Understanding**  
Inspect the structure, categories, distributions, and missingness in the dataset.

**3. Data Preparation**  
Standardise fields, organise categorical variables, remove inconsistencies, and engineer the severity target.

**4. Modelling**  
Train and compare simple models:
- Decision Tree  
- Naïve Bayes  
- K-Nearest Neighbours (KNN)

**5. Evaluation**  
Assess accuracy, confusion matrices, and practical interpretability.

**6. Deployment / Insights**  
Summarise findings, export visuals, and provide a clean notebook for reproducibility.

## Repository Structure
project-1-crispdm-injury-analysis/
│

├ data/ # dataset & metadata

├ notebooks/ # Google Colab notebook

├ scripts/ # helper python scripts (cleaning, EDA, visuals)

├ visuals/ # exported plots

├ docs/ # summaries and CRISP-DM notes

└ README.md # project overview


## Tools and Technologies
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  
- Google Colab  

## How to Run the Notebook (Google Colab)
1. Open the notebook in the `notebooks/` folder.  
2. Mount Google Drive if needed.  
3. Clone the repository in Colab:
   ```python
   !git clone https://github.com/<your-username>/project-1-crispdm-injury-analysis.git
4. Load the dataset from the data/ folder.
5. Run the CRISP-DM sections in order.

# License
This project is licensed under the MIT License.
