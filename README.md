# ML-Health-Care-Premium-Prediction

This project delivers an end-to-end predictive model to estimate health insurance premiums based on factors like age, BMI, smoking habits, income, and medical history. The goal is to help insurance underwriters make accurate premium predictions efficiently through a user-frie

ndly Streamlit web app. The project is divided into two models based on age segmentation and ensures real-time predictions with high precision.

**🔍 Project Overview**

Shield Insurance needed a robust predictive model to streamline its premium estimation process. This project leverages machine learning and data analytics to address the challenge. The core idea was to accurately predict premiums by focusing on demographic, medical, and behavioral factors. Additionally, we performed variance inflation factor (VIF) analysis to handle multicollinearity and created multiple age-segmented models for better prediction.

**🎯 Objective**

The main objectives of this project are:

Build a high-accuracy predictive model (97%+) for health insurance premiums.
Provide real-time predictions via a Streamlit app for underwriters.
Segment the data to improve accuracy by addressing different age groups.
Enable seamless collaboration and cloud deployment for easy access.

**📊 Data Preprocessing and Feature Engineering**

We started by performing thorough Exploratory Data Analysis (EDA) and data preprocessing. This involved the following steps:

1.Data Cleaning:

Handled missing values, outliers, and anomalies in the dataset.
Standardized feature scaling to ensure smooth model performance.

2.Feature Engineering:

Created new features such as Genetical Risk based on health and family history data.
Segmented the data into two groups based on age for better performance:
Model A: For individuals ≤25 years old
Model B: For individuals >25 years old

3.Multicollinearity Check using VIF Analysis:

Used statsmodels.stats.outliers_influence to compute Variance Inflation Factor (VIF).
Removed redundant features to reduce collinearity and improve model robustness.


**🧠 Model Development and Optimization**

We experimented with multiple models, including Linear Regression, Random Forest, and XGBoost, and selected XGBoost due to its superior performance.

Key Highlights:

Segmented models by age group for better precision.
Incorporated additional features for younger groups to boost accuracy.
Performed error analysis to reduce discrepancies between actual and predicted premiums.
Final Results:

Achieved over 97% accuracy.
In 95% of cases, the predicted premium varied by less than 10% from the actual value.

**🌐 Deployment and App Development**

The final models were exported using Joblib and deployed to the cloud for easy access. We built a Streamlit web app to enable underwriters to input variables such as age, income, BMI, smoking habits, and medical history, and receive instant predictions.


App Features:
User-friendly interface for quick premium predictions.
Supports both age-segmented models (≤25 years and >25 years).
Accessible live at: Streamlit App

**🔧 Technology Stack**

Python Libraries: Pandas, NumPy, Scikit-Learn, XGBoost, Joblib
Streamlit: For building an interactive web app
Seaborn & Pandas: For data visualization and EDA
statsmodels: For VIF analysis to detect multicollinearity
GitHub & Cloud Deployment: For version control and accessibility

**🛠 Project Workflow**

Data Cleaning and Preprocessing: Ensured the data was ready for modeling through EDA and VIF analysis.
Feature Engineering: Added additional features and segmented the data.
Model Training and Evaluation: Selected XGBoost for optimal performance and evaluated accuracy metrics.
Model Deployment: Exported the trained models using Joblib and deployed them to the cloud.
Web App Development: Built the final Streamlit app to provide real-time predictions.

**💡 Results and Impact**

The 97%+ accurate model ensures premium predictions are reliable and aligned with business expectations.
The real-time predictions help underwriters make faster, data-driven decisions.
This project has significantly enhanced the efficiency of Shield Insurance’s premium estimation process.

**🔗 Links**
Live App: [Streamlit App](https://healthcarepremiumprediction.streamlit.app/)

GitHub Repository: [ML-Health-Care-Premium-Prediction](https://github.com/Saurabh2535/ML-Health-Care-Premium-Prediction/tree/main)


