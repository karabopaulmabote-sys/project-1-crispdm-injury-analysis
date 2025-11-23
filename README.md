# Workplace Injury Analytics Using the CRISP-DM Lifecycle
This project applies the full Data Science Lifecycle to a workplace injury and illness dataset, following the CRISP-DM framework. The dataset contains claim counts grouped by year, sex, age group, region, employment status, occupation, industry, and injury type. The project forms part of my MEng coursework and focuses on a clear, structured walkthrough of the data science process.

## Objectives
- Understand the structure and behaviour of the dataset  
- Clean, prepare, and organise the data for analysis  
- Explore injury patterns through descriptive analytics  
- Build simple machine learning models (Decision Tree, Naïve Bayes, KNN)  
- Evaluate model performance using standard metrics  
- Present insights that are easy to interpret and grounded in the data  

## CRISP-DM Workflow
**1. Business Understanding**  
Define the purpose of analysing workplace injury data and identify the questions worth answering.

**2. Data Understanding**  
Load the dataset, inspect its structure, categories, missing values, and distributions.

**3. Data Preparation**  
Standardise categories, remove non-informative “Total” rows, encode variables, and prepare numerical fields.

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
