# Project Overview

Cardiovascular disease remains one of the leading causes of mortality worldwide, placing significant pressure on healthcare systems to detect and manage risk early. This project **simulates the work of a data science team within a healthcare technology company** focused on improving cardiovascular risk assessment. This project focuses on building a **data-driven clinical decision support tool** that predicts an individual’s risk of heart disease using machine learning techniques.

From a **business and healthcare analytics perspective**, the goal is to support **early intervention, optimized resource allocation, and improved patient outcomes** by identifying high-risk individuals before critical events occur.

**The Python code covering the full machine learning workflow, from data processing to model development, can be found here [[link](https://github.com/veelvili-tech/Heart-Disease-Prediction-using-Machine-Learning/blob/main/Heart%20Disease%20Prediction%20Using%20Machine%20Learning%20Code.ipynb)].**

# Business Problem

Healthcare providers often rely on a combination of clinical judgment and diagnostic tests to assess heart disease risk. However, these processes can be time-consuming, costly, and reactive.

**Key challenges addressed:**

- Late detection of high-risk patients
- Variability in clinical decision-making
- Limited use of historical patient data for predictive insights

This project demonstrates how **predictive analytics** can complement clinical workflows by delivering **consistent, explainable, and scalable risk assessments.**

# Objective

- Analyze personal and health-related attributes to predict heart disease risk
- Classify patients into high-risk and low-risk categories
- Identify the most influential risk factors to support medical decision-making
- Build a reliable model with ≥85% accuracy and ROC-AUC > 0.90
- Deploy the solution as an interactive application for real-world usability

# Analytical Approach (CRISP-DM)

The project follows the CRISP-DM framework, ensuring a structured and business-aligned workflow:

**1. Business Understanding** – Translating healthcare needs into predictive objectives
**2. Data Understanding** – Exploring patient health indicators and outcome variables
**3. Data Preparation** – Cleaning, standardizing, and selecting relevant features
**4. Modeling** – Comparing multiple supervised learning algorithms
**5. Evaluation** – Selecting the most effective model using robust performance metrics
**6. Deployment** – Delivering insights via a Streamlit web application

<img width="500" height="278" alt="image" src="https://github.com/user-attachments/assets/f03efdb8-3f55-4f10-bd62-b897a4c67e4e" />

# Dataset Overview

- Records: 1,190 patients
- Features: 12 clinical and demographic variables
- Target Variable: Heart disease presence (Yes / No)
- Missing Values: None
- Class Balance:
  - Heart Disease: 52.9%
  - No Heart Disease: 47.1%

The dataset is relatively balanced, enabling reliable model training without aggressive resampling.

# Exploratory Data Analysis – Key Insights
### Risk Drivers Identified

Correlation and feature analysis revealed several medically relevant predictors:

### Strong Positive Correlation with Heart Disease

- Exercise-induced angina
- ST slope
- Oldpeak (ST depression)

### Strong Negative Correlation

- Maximum heart rate achieved

These insights align closely with established clinical knowledge, reinforcing the model’s credibility.

# Data Preparation

- Removed statistically significant outliers
- Standardized numerical features to improve model performance
- Applied Lasso Regression for feature selection to reduce noise and improve interpretability

#Modeling & Evaluation
Multiple supervised learning models were developed and compared:

- Logistic Regression
- Naïve Bayes
- Random Forest
- Support Vector Machine (SVM)
- XGBoost

Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

The final model selection was based on **predictive performance, stability, and business interpretability.**

# Key Business Insights

- Machine learning models can **reliably identify high-risk patients** using routine clinical data
- Tree-based and ensemble models demonstrated superior performance for complex risk patterns
- Feature importance analysis provides **transparent insights** into risk factors, supporting trust among medical professionals

# Deployment & Productization

To demonstrate real-world applicability, the final model was deployed using Streamlit, allowing users to input patient data and receive an immediate risk classification.

# Live Application:
[https://da-heart-disease-prediction-magxjvbgweqhpadsoj6whe.streamlit.app/] 

# Practical Use Cases

- Routine Medical Check-ups: Early identification of high-risk individuals 
- Clinical Triage: Supporting diagnostic prioritization when symptoms are present
- Preventive Healthcare Programs: Targeted lifestyle and treatment interventions

#Tools & Technologies

- Python (Pandas, NumPy, Scikit-learn, XGBoost)
- Data Visualization (Matplotlib, Seaborn)
- Model Explainability (Lasso Regression / SHAP)
- Streamlit for deployment
