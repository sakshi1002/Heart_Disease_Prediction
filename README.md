# Heart Disease Prediction – End-to-End ML Project

An end-to-end Machine Learning project that analyzes, visualizes, and predicts the likelihood of heart disease using clinical and demographic data.

---

## 📌 Project Overview
This project builds a **complete ML workflow** for heart disease prediction:
1. **Exploratory Data Analysis (EDA)** to understand patterns and correlations.
2. **Data cleaning & preprocessing** including handling missing values, encoding categorical features, and feature scaling.
3. **Model development** using multiple machine learning algorithms to classify patients at risk of heart disease.
4. **Model selection & saving** for deployment (using Joblib).

---

## ⚙️ Tech Stack
- **Languages**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Joblib  
- **ML Algorithms**: Logistic Regression, KNN, Naive Bayes, Decision Tree, SVM  

---

## 🔍 Key Steps in Analysis

### 1. Data Exploration & Cleaning
- Loaded dataset (`heart.csv`) with **~900 patient records**.
- Handled missing and duplicate values.
- Replaced `0` cholesterol values with the **mean cholesterol level**.
- Conducted univariate & bivariate analysis with histograms, count plots, and boxplots.

### 2. Feature Engineering & Preprocessing
- One-hot encoded categorical variables (`ChestPainType`, `Sex`, `RestingECG`, etc.).
- Normalized continuous variables (`Age`, `RestingBP`, `Cholesterol`, `MaxHR`, `Oldpeak`) using **StandardScaler**.
- Split dataset into training (80%) and testing (20%).

### 3. Model Training & Evaluation
- Trained and compared **5 ML algorithms**:
  - Logistic Regression  
  - K-Nearest Neighbors (KNN)  
  - Naive Bayes  
  - Decision Tree  
  - Support Vector Machine (SVM)  
- Evaluated models with **Accuracy** and **F1-score**.
- Achieved best performance with **KNN** model.

### 4. Model Deployment
- Saved trained **KNN model**, feature columns, and scaler using **Joblib**:
  - `KNN_heart.pkl`  
  - `scaler.pkl`  
  - `columns.pkl`  

---

## 📊 Business & Health Insights
- Strong correlation between **age, cholesterol, chest pain type, and resting ECG** with heart disease occurrence.
- Patients with **higher cholesterol, abnormal ECG, and chest pain** had significantly higher risk.  
- Predictive modeling achieved **~85% accuracy**, supporting doctors and healthcare providers in **early diagnosis and preventive care**.

---

