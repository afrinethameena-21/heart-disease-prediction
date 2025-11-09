# heart-disease-prediction
# Heart Disease Prediction Using Machine Learning

## Project Overview
This project aims to predict the 10-year risk of Coronary Heart Disease (CHD) using the **Framingham Heart Study dataset**. The goal is to classify whether a patient is likely to develop heart disease (`TenYearCHD = 1`) or not (`TenYearCHD = 0`) based on clinical and demographic features.

---

## Dataset
- **Source:** Framingham Heart Study dataset  
- **Features Used:**  
  - `age`: Age of the patient  
  - `Sex_male`: Gender (1 = Male, 0 = Female)  
  - `cigsPerDay`: Number of cigarettes smoked per day  
  - `totChol`: Total cholesterol (mg/dL)  
  - `sysBP`: Systolic blood pressure  
  - `glucose`: Blood glucose level  
- **Target:** `TenYearCHD` (0 = No, 1 = Yes)  

**Data Preprocessing Steps:**  
1. Dropped the `education` column (not used in model).  
2. Handled missing values by removing rows with `NaN`.  
3. Standardized features using `StandardScaler` to normalize scale differences.

---

## Approach
1. **Data Splitting:**  
   - Train/Test split: 70% training, 30% testing  
   - Random state = 4 for reproducibility  

2. **Model Used:**  
   - **Logistic Regression** (baseline interpretable model)  
   - Alternative explored: Random Forest (non-linear relationships and feature importance)  

3. **Model Training & Prediction:**  
```python
from sklearn.linear_model import LogisticRegression

logreg = LogisticRegression()
logreg.fit(X_train, y_train)
y_pred = logreg.predict(X_test)
