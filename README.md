\## 🩺 \*\*Diabetes Prediction Using Machine Learning\*\*



\### \*\*Project Overview\*\*



Diabetes is one of the most prevalent chronic diseases worldwide and early diagnosis is critical for preventing severe health complications. This project develops and evaluates machine learning models capable of predicting the probability of diabetes diagnosis using demographic, lifestyle, and clinical indicators.



The study addresses a highly imbalanced healthcare dataset and compares the performance of Logistic Regression and Random Forest classifiers to identify the most reliable predictive framework for diabetes risk assessment.



\### \*\*Objectives\*\*

* Perform comprehensive data cleaning and preprocessing.
* Conduct exploratory data analysis (EDA) to uncover key risk factors associated with diabetes.
* Build and compare multiple machine learning classification models.
* Optimize model performance using hyperparameter tuning and cross-validation.
* Develop a predictive framework capable of supporting early diabetes screening and risk assessment.



\### \*\*Dataset Description\*\*

The dataset contains demographic, lifestyle, and clinical information from over 100,000 patients.



\#### \*\*Features\*\*

* Gender
* Age
* Hypertension
* Heart Disease
* Smoking History
* Body Mass Index (BMI)
* HbA1c Level
* Blood Glucose Level

\#### \*\*Target Variable\*\*

\*\*Diabetes Status\*\*

\*\*0\*\* = Non-Diabetic

\*\*1\*\* = Diabetic



\#### \*\*Class Distribution\*\*

Non-Diabetic: 91.2%

Diabetic: 8.8%



The substantial class imbalance required the implementation of class-weighted machine learning techniques to ensure effective identification of diabetic patients.



\### \*\*Exploratory Data Analysis\*\*



Key insights obtained during exploratory analysis include:



\#### \*\*Clinical Indicators\*\*

* \*\*HbA1c Level\*\* showed a strong positive association with diabetes (r = 0.41).
* \*\*Blood Glucose Level\*\* exhibited the highest correlation with diabetes diagnosis (r = 0.42).
* Diabetic patients recorded substantially higher average glucose concentrations and HbA1c levels than non-diabetic individuals.



\#### \*\*Demographic Factors\*\*

Diabetes prevalence increased significantly with age.

* \*\*Middle-aged\*\* and \*\*older adults\*\* exhibited the highest diagnosis rates.
* Female patients represented a larger proportion of the dataset population.



\#### \*\*Comorbidities\*\*

* \*\*28%\*\* of hypertensive individuals were diagnosed with diabetes.
* \*\*32.3%\*\* of individuals with heart disease were diabetic.
* Diabetes prevalence was considerably lower among individuals without these conditions.

Lifestyle Factors

* Former smokers demonstrated the highest diabetes prevalence among smoking categories, suggesting a strong association between smoking history and diabetes risk.



\### \*\*Machine Learning Models\*\*

\#### \*\*Logistic Regression (Baseline Model):\*\* A class-weighted Logistic Regression model was implemented as the baseline classifier.



\#### \*\*Random Forest Classifier:\*\* A Random Forest model was developed and optimized using:

* GridSearchCV
* Cross-validation
* Hyperparameter tuning
* Class balancing techniques
* 

\### \*\*Model Performance\*\*

Random Forest (Test Set)

!\[ROC Curve](visuals/roc\_curve.png)



!\[Confusion Matrix](visuals/confusion\_matrix.png)



!\[Correlation Heatmap](visuals/correlation\_heatmap.png)



!\[Comparison of Models](visuals/model\_performance.png)



The optimized Random Forest Classifier outperformed Logistic Regression across all major evaluation metrics.



\#### \*\*Key achievements include:\*\*



* ROC-AUC of 0.97
* Recall of 0.89
* Accuracy of 91%
* Only 185 diabetic patients missed in the testing dataset



The model successfully balances predictive performance with clinical relevance by prioritizing the detection of diabetic patients.



\### \*\*Key Findings\*\*

* Blood Glucose Level and HbA1c Level emerged as the strongest predictors of diabetes diagnosis.
* Diabetes prevalence increases substantially with age.
* Hypertension and heart disease are strongly associated with diabetes risk.
* Former smokers exhibit elevated diabetes prevalence compared to other smoking categories.
* Random Forest effectively captures complex nonlinear relationships among clinical risk factors.



\### \*\*Technologies Used\*\*

* Python
* Pandas
* NumPy
* Scikit-Learn
* SciPy
* Matplotlib
* Seaborn
* Plotnine



\### \*\*Project Structure\*\*

Diabetes-Prediction/

│

├── data/

├── notebooks/

├── visuals/

├── models/

├── README.md

