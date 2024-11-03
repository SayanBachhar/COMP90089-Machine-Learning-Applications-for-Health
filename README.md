# README

There are 2 code files present:
+ **Dataset_Generation.ipynb** - Access MIMIC-IV database, find a subset of patients who have been diagnosed with pneumonia. Get all their medical details - demographics, comorbidities, medications, lab events, chart events. Also, add if the patient has a diagnosis of heart failure within the next 6 months. Output the details to *"final_patients_dataset.csv"*

+ **ML_Code.ipynb** - Perform data preprocessing and run various models with the patients data in above generated csv file. Some operations involve filling missing values, scaling the data, doing RFE (Recursive Feature Elimination) for feature selection, run multiple ML models, hyperparameter tuning and various visualisations. The main models that were trained and tested on were - Logistic Regression, Decision Tree, Random Forest, AdaBoost, XGBoost, Support Vector Classifier. The main visuals were bar charts and SHAP.

## Instructions

Before running the "Dataset_Generation.ipynb" file, make sure to first upload it to Google Colab, change the "project_id" variable in the file to the one associated with MIMIC-IV in your colab environment and then run it.

Before running the "ML_Code.ipynb" file, especially if trying to do it locally, make sure to run the "requirements.txt" file to install the relevant python libraries. Do this by calling the following command:\
`pip install -r requirements.txt`

Note: The python used for testing was **Python 3.12.5**