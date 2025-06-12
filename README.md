# Task-3-Disease-Diagnosis-Prediction-

**Objective:**

* Build a machine learning model to predict the likelihood of diabetes using medical data and provide insights for early diagnosis.

**Dataset:**
**Source**: [PIMA Indians Diabetes Dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv)


* Features: Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age
* Target: Outcome (1 = Diabetes, 0 = No Diabetes)

**Steps Overview:**

1. **Import Libraries & Load Dataset**

   * Installed: pandas, numpy, scikit-learn, matplotlib, seaborn
   * Loaded dataset from URL using pandas

2. **Exploratory Data Analysis (EDA)**

   * Used correlation heatmap to identify feature relationships
   * Found strong correlation of Glucose and BMI with diabetes outcome

3. **Preprocessing & Feature Scaling**

   * Separated features (X) and target (y)
   * Scaled features using StandardScaler
   * Split data into training and testing sets (80/20)

4. **Model Training**

   * Trained three models:

     * Gradient Boosting
     * Support Vector Machine (SVM)
     * Neural Network (MLPClassifier)

5. **Model Evaluation**

   * Evaluated using:

     * F1 Score
     * AUC-ROC Curve
   * Gradient Boosting showed best performance:

     * F1 Score: 0.65
     * AUC: 0.81

6. **Feature Importance (Gradient Boosting)**

   * Top features:

     * Glucose
     * BMI
     * Age
     * DiabetesPedigreeFunction

7. **Insights for Healthcare Professionals**

   * Key predictors of diabetes: Glucose, BMI, Age, Pedigree
   * Focus on monitoring glucose and BMI regularly
   * Give attention to older patients or those with family history
   * Gradient Boosting model suitable for early detection tools



**Outcome:**

* A working prediction model to assist healthcare professionals
* Enables early identification of high-risk individuals
* Provides explainable results using feature importance analysis
