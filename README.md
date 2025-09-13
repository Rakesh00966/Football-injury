# 🏟️ Football Injury Prediction using Logistic Regression
[GITHUB LINK](https://github.com/Rakesh00966/Football-injury/blob/main/Football_injury_prediction.ipynb)

This project focuses on predicting whether a football player will face an injury in the next season using **machine learning (Logistic Regression)**.  
The dataset contains player information such as age, physical attributes, training workload, past injuries, fitness test scores, sleep, stress levels, and more.  

---

## 📌 Project Overview
- **Goal:** Predict the target variable `Injury_Next_Season` (0 = No Injury, 1 = Injury).  
- **Dataset Size:** 800 players  
- **Features:** 19 (Age, Height, Weight, Position, Training Hours, Previous Injury Count, BMI, etc.)  
- **Target:** `Injury_Next_Season` (binary classification)

---

## 🛠️ Steps Performed
1. **Exploratory Data Analysis (EDA)**
   - Checked distributions of features like Age, Training Hours, Stress Level, BMI, etc.
   - Visualized injury distribution across player positions.
   - Analyzed correlations between variables (e.g., Stress Level & Reaction Time had strong influence).

2. **Data Preprocessing**
   - Encoded categorical column `Position` using **One-Hot Encoding**.
   - Standardized numerical features using **StandardScaler**.

3. **Model Building**
   - Trained a **Logistic Regression model**.
   - Split data into **80% training** and **20% testing**.

4. **Model Evaluation**
   - Achieved high accuracy on both training and test sets.
   - Evaluated using:
     - Accuracy Score
     - Classification Report
     - Confusion Matrix

---

## 📊 Results
**Training Performance:**
- Accuracy: **96.5%**
- Confusion Matrix:  
 [[309  11]
 [ 11 309]]


**Testing Performance:**
- Accuracy: **93.7%**
- Confusion Matrix:  
 [[72  8]
 [ 2 78]]


---

## 🚀 Key Insights
- Stress Level and Reaction Time had the highest positive correlation with future injuries.
- BMI was strongly related to weight (as expected).
- Training Hours, Matches Played, and Age were less influential compared to flexibility, sleep, and stress scores.

---

## 📦 Tech Stack
- **Python** (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Machine Learning Algorithm:** Logistic Regression

---

## 📌 Future Improvements
- Try other models (Random Forest, XGBoost, Neural Networks).
- Perform Hyperparameter Tuning for better generalization.
- Include feature selection & cross-validation.
- Build a web dashboard for interactive injury predictions.
