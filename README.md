# 🏥 Post-AMI 30-Day Mortality Prediction

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 📌 Project Overview
Accurate risk stratification after Acute Myocardial Infarction (AMI) is essential for guiding clinical decision-making. This project develops and internally validates a parsimonious prediction model for 30-day mortality using routinely available clinical data from 785 patients.

**Key Achievements:**
- Cleaned and handled missing values across clinical variables using median/mode imputation.
- Utilized **LASSO Logistic Regression** for feature selection and regularization to handle low events-per-variable.
- Achieved a **Test AUC of 0.87**, identifying Age, Killip Class, Heart Rate, and Previous MI as the strongest predictors of mortality.
- Evaluated clinical utility using **Decision Curve Analysis (DCA)**, demonstrating net clinical benefit at threshold probabilities between 5% and 35%.

## 📂 Repository Structure
- `Post_AMI_Mortality_prediction.ipynb`: The Jupyter Notebook containing the full Exploratory Data Analysis (EDA), data cleaning, and modeling pipeline.
- `Post_AMI_Mortality_Report.pdf`: The final academic report detailing the methodology, calibration plots, DCA, and clinical conclusions.
- `report_source.tex`: The LaTeX source code for the report.
- `data/`: Contains the anonymized clinical dataset used for training and testing the model.

## 🛠️ Methodology & Tech Stack
- **Data Preprocessing:** Addressed data entry errors, mapped categorical variables, and performed stratified Train/Test splitting (80/20).
- **Modeling:** SimpleImputer, StandardScaler, and Hyperparameter tuning via `GridSearchCV` for optimizing the LASSO regularization penalty.
- **Libraries Used:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`.

## 🚀 How to Explore
1. You can view the full code, visualizations, and outputs directly by clicking on the `Post_AMI_Mortality_prediction.ipynb` file above.
2. For a detailed breakdown of the statistical methods and clinical interpretation, please read the `Post_AMI_Mortality_Report.pdf`.
3. To run the code locally, clone the repository and ensure the anonymized dataset is placed in the `data/` directory.
