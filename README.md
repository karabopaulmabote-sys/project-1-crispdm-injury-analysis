# Incident Severity Classification Using CRISP-DM

This project forms part of my MEng coursework and demonstrates the complete Data Science Lifecycle using the CRISP-DM framework. The goal was to classify workplace accident severity into three levels based on incident type, industry, and the recorded injuries and fatalities. The project uses publicly available occupational accident data and focuses on applying a structured, end-to-end workflow rather than building highly optimised models.

## 1. Business Understanding

Incident investigations often produce unstructured information that is difficult to analyse consistently. This project aimed to turn incident characteristics into structured features and model incident severity as a three-class problem:

- **Low severity:** no injuries and no fatalities  
- **Moderate severity:** injuries but no fatalities  
- **High severity:** incidents involving fatalities or multiple injuries  

The project explores whether simple machine learning models can classify incidents using only a small set of features.

## 2. Data Understanding

The dataset includes:

- Incident title and description  
- Province  
- Industry  
- Incident type  
- Number of injuries (categorical ranges)  
- Number of deaths (categorical ranges)  
- Financial penalties and enforcement outcomes  

Initial inspection showed several categorical fields, a small number of missing values, and injury/fatality fields encoded as ranges.

## 3. Data Preparation

Key preparation steps:

- Dropped unused fields (`city`, `sub industry`, `company name`, `company ownership`)  
- Removed rows with missing incident type  
- Converted injury and fatality ranges to ordinal values  
- Engineered a three-class severity label based on the injury and fatality structure  
- One-hot encoded all categorical fields for modelling  

This created a clean, usable dataset containing both categorical and ordinal variables.

## 4. Exploratory Data Analysis (EDA)

The EDA focused on:

- Severity distribution  
- Incident types and industries with the highest counts  
- Relationships between injuries, fatalities, and severity  
- Correlations between engineered features  

**Key insights:**

- Severity is driven mainly by fatalities and, to a lesser extent, injury counts.  
- Construction, mining, and industrial sectors show higher concentrations of severe incidents.  
- Certain incident types (fires, structural failures, mechanical accidents, transport accidents) appear frequently across all severity levels.  
- The engineered severity classes are well-separated in the data.

## 5. Modelling

Three baseline classifiers were trained:

- Decision Tree  
- Naïve Bayes (Multinomial)  
- K-Nearest Neighbours (k=5)

All models used a shared preprocessing pipeline with One-Hot Encoding.

### Performance Summary

| Model | Accuracy |
| **Decision Tree** | **1.00** |
| Naïve Bayes | 0.893 |
| KNN (k=5) | 0.857 |

The Decision Tree achieved perfect accuracy on the test set, reflecting the clear, rule-based structure of the engineered severity classes and the strong signal carried by injury and fatality counts. Naïve Bayes and KNN performed well overall but struggled more with the moderate severity class, which is the smallest and most variable group.

## 6. Conclusions

Working through the CRISP-DM phases provided a structured way to approach the project. The preparation work showed how important it is to turn real-world fields into meaningful numerical representations. The EDA confirmed expected patterns in safety-related data, and the modelling process demonstrated that simple classifiers can perform effectively when the features are well-defined.
"""

## Repository Structure
project-1-crispdm-injury-analysis/
│

├ data/ 
   ├ accidents.csv
   └ README.md
│
├ notebooks/ 
   └ incident_severity.ipynb
│
├ requirements.txt

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
