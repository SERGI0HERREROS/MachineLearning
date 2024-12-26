# MachineLearning 24-25
**Repository for the practices of the subject Machine Learning**

## 🤗 Authors

| Name                          | Github user                                        |
|-------------------------------|----------------------------------------------------|
| Sergio Herreros Fernández     | [@SergioHerreros](https://github.com/SERGI0HERREROS)
| Francisco Javier Luna Ortiz   | [@Lunao01](https://github.com/Lunao01)
| Carlos Romero Navarro         | [@KarManiatic](https://github.com/KarManiatic)
| Tatsiana Shelepen             | [@Naschkatzee](https://github.com/Naschkatzee)                 
<br>

## 🎯 Problem description
The goal of this project is to predict the probability that people receive two types of vaccines:
- H1N1 flu vaccine.
- Seasonal flu vaccine.

All the information is on the following site:<br>
https://www.drivendata.org/competitions/66/flu-shot-learning/page/210/
<br><br>



## 🚩 Labels
There are two target variables:
- **h1n1_vaccine** - Whether respondent received H1N1 flu vaccine.
- **seasonal_vaccine** - Whether respondent received seasonal flu vaccine.

Both are binary variables: 0 = No; 1 = Yes.
<br><br>



## 🗒️ Features
List of features:

- **h1n1_concern** - Level of concern about the H1N1 flu.
    - 0 = Not at all concerned; 1 = Not very concerned; 2 = Somewhat concerned; 3 = Very concerned.

- **h1n1_knowledge** - Level of knowledge about H1N1 flu.
    - 0 = No knowledge; 1 = A little knowledge; 2 = A lot of knowledge.

- **behavioral_antiviral_meds** - Has taken antiviral medications. (binary)

- **behavioral_avoidance** - Has avoided close contact with others with flu-like symptoms. (binary)

- **behavioral_face_mask** - Has bought a face mask. (binary)

- **behavioral_wash_hands** - Has frequently washed hands or used hand sanitizer. (binary)

- **behavioral_large_gatherings** - Has reduced time at large gatherings. (binary)

- **behavioral_outside_home** - Has reduced contact with people outside of own household. (binary)

- **behavioral_touch_face** - Has avoided touching eyes, nose, or mouth. (binary)

- **doctor_recc_h1n1** - H1N1 flu vaccine was recommended by doctor. (binary)

- **doctor_recc_seasonal** - Seasonal flu vaccine was recommended by doctor. (binary)

- **chronic_med_condition** - Has any of the following chronic medical conditions: asthma or an other lung condition, diabetes, a heart condition, a kidney condition, sickle cell anemia or other anemia, a neurological or neuromuscular condition, a liver condition, or a weakened immune system caused by a chronic illness or by medicines taken for a chronic illness. (binary)

- **child_under_6_months** - Has regular close contact with a child under the age of six months. (binary)

- **health_worker** - Is a healthcare worker. (binary)

- **health_insurance** - Has health insurance. (binary)

- **opinion_h1n1_vacc_effective** - Respondent's opinion about H1N1 vaccine effectiveness.
    - 1 = Not at all effective; 2 = Not very effective; 3 = Don't know; 4 = Somewhat effective; 5 = Very effective.

- **opinion_h1n1_risk** - Respondent's opinion about risk of getting sick with H1N1 flu without vaccine.
    - 1 = Very Low; 2 = Somewhat low; 3 = Don't know; 4 = Somewhat high; 5 = Very high.

- **opinion_h1n1_sick_from_vacc** - Respondent's worry of getting sick from taking H1N1 vaccine.
    - 1 = Not at all worried; 2 = Not very worried; 3 = Don't know; 4 = Somewhat worried; 5 = Very worried.

- **opinion_seas_vacc_effective** - Respondent's opinion about seasonal flu vaccine effectiveness.
    - 1 = Not at all effective; 2 = Not very effective; 3 = Don't know; 4 = Somewhat effective; 5 = Very effective.

- **opinion_seas_risk** - Respondent's opinion about risk of getting sick with seasonal flu without vaccine.
    - 1 = Very Low; 2 = Somewhat low; 3 = Don't know; 4 = Somewhat high; 5 = Very high.
    
- **opinion_seas_sick_from_vacc** - Respondent's worry of getting sick from taking seasonal flu vaccine.
    - 1 = Not at all worried; 2 = Not very worried; 3 = Don't know; 4 = Somewhat worried; 5 = Very worried.

- **age_group** - Age group of respondent.

- **education** - Self-reported education level.

- **race** - Race of respondent.

- **sex** - Sex of respondent.

- **income_poverty** - Household annual income of respondent with respect to 2008 Census poverty thresholds.

- **marital_status** - Marital status of respondent.

- **rent_or_own** - Housing situation of respondent.

- **employment_status** - Employment status of respondent.

- **hhs_geo_region** - Respondent's residence using a 10-region geographic classification defined by the U.S. Dept. of Health and Human Services. Values are represented as short random character strings.

- **census_msa** - Respondent's residence within metropolitan statistical areas (MSA) as defined by the U.S. Census.

- **household_adults** - Number of other adults in household, top-coded to 3.

- **household_children** - Number of children in household, top-coded to 3.

- **employment_industry** - Type of industry respondent is employed in. Values are represented as short random character strings.

- **employment_occupation** - Type of occupation of respondent. Values are represented as short random character strings.
<br><br>


## 🧩 Project Structure

### / (Root Directory)  
The main folder of the project.  

---

### **best_models/**  
Contains the best-performing models.  
- **`HistGradientBoosting.ipynb`**: Notebook for HistGradientBoosting model.  
- **`RandomForest_with_partition.ipynb`**: Notebook for Random Forest with partitions.  
- **`Summary_Results.txt`**: Text file summarizing key results.  

---

### **data/**  
Stores project data.  
- **`gold/`**: Final, processed datasets.  
- **`raw/`**: Unprocessed, raw data.  

---

### **EDAs/**  
Notebooks for exploratory data analysis (EDA).  
- **`Exploratory data analysis_changes.ipynb`**: Updated or modified analysis.  
- **`Exploratory data analysis.ipynb`**: Initial EDA notebook.  

---

### **other_models/**  
Notebooks for additional models.  
- **`Decision Tree imputation.ipynb`**: Decision Tree with data imputation.  
- **`Decision Tree.ipynb`**: Basic Decision Tree model.  
- **`KNN(Estimators).ipynb`**: K-Nearest Neighbors model.  
- **`LogisticRegression.ipynb`**: Logistic Regression model.  
- **`RandomForest.ipynb`**: Random Forest model.  

---

### **profiling/**  
Contains profiling results.  
- **`report.html`**: HTML file with data profiling report.  

---

### **results/**  
Outputs generated by models in CSV format.  
- **`pred_decision_tree_impute_output.csv`**: Predictions from Decision Tree with imputation.  
- **`pred_decision_tree_output.csv`**: Predictions from standard Decision Tree.  
- **`pred_hist_gradient_boosting.csv`**: Predictions from HistGradientBoosting.  
- **`pred_KNN_output.csv`**: Predictions from KNN.  
- **`pred_logistic_regression_output.csv`**: Predictions from Logistic Regression.  
- **`pred_random_forest_output.csv`**: Predictions from Random Forest.  

---

### **PROJECT_STRUCTURE.txt**  
This file explains the structure of the project, detailing the purpose of each folder and file for better understanding and navigation.  

---

### **README.md**  
Project description.  
