# Supervised--ML--Classification
**CARDIOVASCULAR RISK PREDICTION.**

**Problem Statement:**
The dataset is from the ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of coronary heart disease(CHD). The dataset provides the patient's information . It includes 3390 records and 16 attributes. Each attribute is a potental risk factor having demographic, behavioral, and medical attributes.

**Project Summary:**
The Cardiovascular Risk Prediction dataset includes data on 3,390 patients, featuring 16 predictor variables and 1 target variable. Each variable represents a potential risk factor, including demographic, behavioral, and medical factors. Our objective is to predict the likelihood of developing coronary heart disease (CHD) over a 10-year period.

Key steps taken and approach towards our target problem:

1. **Data Gathering and Cleaning:** We started by gathering the dataset, which contains 3390 records and 16 attributes. We performed data cleaning, handling null values, checking data distribution, and handling outliers to ensure data quality.

2. **Exploratory Data Analysis(EDA):** In this phase, we conducted an in-depth analysis of the dataset. We employed various visualization techniques, separating them into univariate, bivariate categories. Through EDA, we gained meaningful insights that guided our decision-making for the subsequent steps 

3. **Feature Engineering and Data Preprocessing:**  We performed feature engineering to extract new features that could potentially impact the prediction of the 10-year CHD risk. Additionally, we addressed multicollinearity among independent variables using the Variance Inflation Factor (VIF). Categorical features were encoded into numerical values using binary label encoding.

4. **Data Transformation:**  To achieve normally distributed data, we applied Logarithmic transformations. Additionally, we employed the StandardScaler from the sklearn library to scale the data.

5. **Handling Class Imbalance:** The distribution of the target variable, TenYearCHD, was found to be imbalanced, with only 15% of individuals classified as having a high risk of developing CHD. To address this issue, we employed the Synthetic Minority Oversampling Technique (SMOTE) to create a balanced dataset.

6. **Model Implementation:**  We split the data into train and test sets, and evaluated several classification models, including Logistic Regression, Random Forest, XGBoost, KNN, and SVM. Various metrics such as Precision, Recall, F1 Score, Accuracy, and AUC-ROC were compared using classification reports and confusion matrices. Considering our objective of reducing false negatives, emphasizing Recall was essential. After thorough experimentation, XGBoost emerged as the optimal model, achieving the highest metrics overall.

7. **Model Deployment:**  Based on our evaluations and comparisons, we selected XGBoost as our final model for deployment. This model, fine-tuned with a learning rate of 0.1, maximum tree depth of 7, and 170 trees, demonstrated superior Recall(85%), Precision(91%), F1 Score(88%), Accuracy(89%), and AUC-ROC(94%) scores.

In conclusion, this project with various machine learining algorithm helps the medical community to build diagnostic tool to predict the risk fo 10 year CHD.By our all steps taken combining data processing, feature engineering, model evaluation, and selection, we successfully built an accurate model capable of identifying potential CHD patients in the future.
