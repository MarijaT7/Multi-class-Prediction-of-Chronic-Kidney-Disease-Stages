# Multi-class-Prediction-of-Chronic-Kidney-Disease-Stages
Projekat na predmetu Mašinsko učenje 1.
# Project Overview
This project focuses on the risk assessment and stage classification of Chronic Kidney Disease (CKD) using a comprehensive dataset of clinical, lifestyle, and familial characteristics. The goal is to develop a machine learning model capable of performing multi-class classification to categorize patients into one of five distinct stages: No_Disease, Low_Risk, Moderate_Risk, High_Risk, Severe_Disease. 
# Dataset Analysis
The project utilizes the Kidney Disease Dataset from Kaggle : https://www.kaggle.com/datasets/amanik000/kidney-disease-dataset. Samples: 20,538, Features: 43 initial features (reduced to 41 after preprocessing). Data Composition: 27 numerical features.Target Variable: Multi-class (5 categories). 
# Sample Representation 
Each sample represents an individual patient's profile, including medical metrics (e.g., Blood Pressure, Creatinine, eGFR), demographic data, lifestyle habits (e.g., smoking, physical activity), and family medical history.
# Preprocessing & Feature Engineering
Missing Values: The dataset was found to be clean with 0% missing values. 
Feature Selection: 1. Removed Specific Gravity and Urine Albumin due to low variability and non-standard clinical representation in this specific set. 
                   2. Removed Cystatin C, Serum Albumin, Serum Calcium, and Serum Potassium based on variance analysis (limited discriminative power). 
Outlier Handling: High values in Serum Creatinine were identified; however, they were retained as valid pathological data essential for detecting severe kidney dysfunction.
Class Imbalance: The dataset is highly imbalanced, with the No_Disease class making up ~80% of the data, while Severe_Disease accounts for only ~2%. 
# Key Features Included
The model processes a wide range of indicators, including: 
Clinical: Blood Pressure, Glucose, Hemoglobin, eGFR, Creatinine, CRP levels, etc. 
Behavioral: Smoking status, Physical activity level, BMI. 
Familial: Family history of Chronic Kidney Disease. 
Comorbidities: Hypertension, Diabetes Mellitus, Coronary Artery Disease.
