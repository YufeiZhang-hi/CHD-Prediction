# **Coronary Heart Disease Prediction** 

### **Overview**
This project demonstrates a full data analytics workflow—from data preprocessing and feature engineering to model training, evaluation, and Google Cloud deployment. The goal is to predict an individual's risk of Coronary Heart Disease (CHD) over a specified period using structured health data.  

---  

### **Features**  

#### **Exploratory Data Analysis**  
- **Tableau** – Created **interactive dashboards** to explore key trends, feature importance, and risk factors.  

#### **Data Processing**  
- Missing Value Imputation  
- Outlier Treatment – Applied **log transformations** to skewed variables.  
- Feature Engineering:  
  - Encoded categorical variables using **one-hot encoding and label encoding**.  
  - Selected or removed features based on **correlation analysis**.  
  - Used **SMOTE** to balance the dataset.

#### **Model Training**  
- Algorithms Used – Trained **Logistic Regression, SVM, Random Forest, and XGBoost**.  
- Ensemble Learning – Combined models using a **voting classifier** to improve prediction stability.  
- Model Validation – Evaluated model performance using **Accuracy, F1-Score, and AUC-ROC metrics**.  

#### **Deployment**  
- **Google Cloud Integration**:  
  - Training & Inference Pipelines – Automated workflows using **Kubeflow Pipelines**.  
  - Cloud Storage & AI Platform – Deployed the final model to **Google Cloud Platform**, enabling real-time predictions via an **API**.

---  

### **Project Components**  
- **`CHD_Model_Training.ipynb`** – Full pipeline for data processing, feature engineering, model training, and evaluation.  
- **`CHD_Model_Inference.ipynb`** – Loads the trained model, processes new patient data, and makes real-time predictions.  
- **`CHD_Model_Training.json`** – Defines the automated training pipeline for **Kubeflow**.  
- **`CHD_Model_Inference.json`** – Specifies the inference pipeline for making predictions on new patient data.  
- **`CHD_EDA_Dashboard.twb`** – Tableau workbook for data exploration and visualization.  

---  

### **Key Features**  
- End-to-End Pipeline – Covers data ingestion, preprocessing, model training, and inference.  
- Model Optimization – Used cross-validation, achieving **73.62% accuracy and 73.93% F1-score**.  
- Cloud Deployment – Deployed the trained model on Google Cloud Platform for real-time predictions.  
- Interactive Data Visualization – Built dynamic dashboards in Tableau to provide actionable insights on CHD risk factors.  

