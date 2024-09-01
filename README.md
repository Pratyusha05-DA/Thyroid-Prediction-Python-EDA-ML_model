## **Thyroid Cancer Recurrence Prediction**
This project focuses on predicting the recurrence of thyroid cancer by analyzing clinical and demographic data using machine learning. The primary goal is to create a predictive model that helps healthcare professionals make informed decisions, ultimately improving patient outcomes.

### **Project Overview**
Thyroid cancer is one of the most common endocrine malignancies, and predicting its recurrence is crucial for effective patient management. In this project, we used a dataset containing information on 383 patients, including various clinical and demographic factors such as age, gender, smoking history, adenopathy, and cancer stage. The project leverages a Random Forest Classifier to predict whether a patient is likely to experience a recurrence of thyroid cancer.

### **Objectives**
* **Prediction**: Develop a machine learning model to accurately predict thyroid cancer recurrence.
* **Insight Generation**: Identify the most significant factors contributing to cancer recurrence.
* **Clinical Application**: Provide insights that can be used to tailor patient care and reduce recurrence rates.

### **Data and Features**
The dataset comprises 383 patient records with 17 features. The analysis focused on the following key columns:

* Age: Patient’s age at the time of diagnosis.
* Gender: Male or female.
* Smoking History: Whether the patient has a history of smoking.
* Adenopathy: Involvement of lymph nodes (e.g., extensive, left, right).
* Cancer Stage: TNM staging of the cancer.
* Response: Response to initial treatment.
* Thyroid Function: Clinical status of the thyroid (e.g., hypothyroidism, euthyroid).
* Recurred: Target variable indicating recurrence (Yes/No).
These features were carefully selected and processed to ensure that the model captures the most relevant information for predicting cancer recurrence.

### **Methodology**
#### Data Preparation
Data preparation involved several critical steps:

* **Cleaning**: We removed any missing values and handled outliers to ensure data quality.
* **Feature Engineering**: New features were created based on existing data, such as:
* **Age_Above_60**: A binary feature indicating whether the patient is older than 60 years.
* **Risk Categories**: Simplified risk categories based on the combination of cancer stage and lymph node involvement.

### **Analysis and Model Building**
##### **Statistical Analysis**:

* **Chi-square Test**: Performed to examine the relationship between categorical variables (e.g., Gender, Smoking History) and the target variable (Recurred). This test helped identify significant associations between these features and cancer recurrence.
* **T-test**: Applied to compare the means of numerical features (e.g., Age) between patients who experienced recurrence and those who did not. The T-test determined whether the differences in age groups were statistically significant.
##### **Model Building**:

We employed a Random Forest Classifier, a robust and versatile machine learning model, to predict cancer recurrence. This model was chosen for its ability to handle complex datasets and its high accuracy.
Model Performance: The model achieved a 97% accuracy rate, with a precision of 95%, making it a reliable tool for predicting thyroid cancer recurrence

### **Key Findings**
* **Recurrence Rate**: Approximately 28.2% of patients experienced cancer recurrence.
* **Age and Gender**: Patients who experienced recurrence tended to be older on average, with a higher recurrence rate observed in males.
* **Significant Predictors**: Features such as smoking history, adenopathy, cancer stage, and response to treatment showed significant correlations with cancer recurrence.
* **Model Performance**: The Random Forest model achieved an accuracy of 96%, with high precision and recall, indicating its effectiveness in predicting thyroid cancer recurrence.

### **Conclusion**
This project demonstrates the power of machine learning in healthcare, specifically in predicting thyroid cancer recurrence. The Random Forest Classifier developed here is not only accurate but also provides valuable insights into the factors that influence cancer recurrence. These findings can be used to enhance patient care, tailor treatment plans, and ultimately improve outcomes for patients with thyroid cancer.
