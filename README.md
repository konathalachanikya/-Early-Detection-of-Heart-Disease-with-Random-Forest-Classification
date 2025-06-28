# -Early-Detection-of-Heart-Disease-with-Random-Forest-Classification

Predicting heart disease using clinical health records with a supervised learning approach. This project demonstrates how machine learning can assist in early diagnosis and preventive care for cardiovascular patients.

---

## 📊 Project Overview

This project uses the **Heart Disease UCI dataset** to build a predictive model that classifies whether a patient has heart disease based on clinical features. The goal is to assist healthcare professionals with a reliable tool for early detection and screening.

---

## 🧠 Problem Statement

> Can we accurately predict the presence of heart disease using patient vitals such as age, cholesterol, chest pain type, blood pressure, and more?

---

## 📁 Dataset Details

- **Source**: [Kaggle – Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- **Records**: 1,025 patient entries
- **Features**:
  - Age, Sex, Chest Pain Type (cp)
  - Resting Blood Pressure (trestbps)
  - Cholesterol (chol)
  - Maximum Heart Rate Achieved (thalach)
  - ST Depression (oldpeak)
  - Exercise Induced Angina (exang)
- **Target Variable**: `target` (0 = No disease, 1 = Heart disease)

---

## 🔄 ML Workflow

### 1. Data Collection
Loaded dataset using `pandas`.

### 2. Data Preparation
- Removed missing/invalid values
- Scaled numeric features using `StandardScaler`

### 3. Exploratory Data Analysis (EDA)
- Plotted survival distribution, cholesterol vs target, age vs heart rate
- Key correlation trends identified

### 4. Feature Engineering
- Selected key predictors based on medical relevance and model importance

### 5. Model Training
- Algorithms Used: `RandomForestClassifier`, `LogisticRegression`
- 80/20 train-test split with stratified sampling

### 6. Evaluation
- Achieved **~85% accuracy** on test data
- Balanced precision and recall
- Interpretable feature importance chart

---

## 📈 Results & Interpretation

Top predictive features:
- Chest Pain Type (`cp`)
- ST Depression (`oldpeak`)
- Max Heart Rate (`thalach`)
- Cholesterol (`chol`)
- Exercise-Induced Angina (`exang`)

These align with known cardiology risk factors, validating the model's reliability.

---

## 💼 Business Insights

- Focus early testing on patients aged 50+ with abnormal chest pain and low `thalach`
- Integrate ML predictions into hospital triage systems for faster diagnosis
- Can assist in rural healthcare, telemedicine, and insurance risk scoring

---

## 📂 Files

| File | Description |
|------|-------------|
| `heart.csv` | Dataset file |
| `Heart_Disease_Prediction_KChanikya.ipynb` | Full Jupyter Notebook |
| `Heart_Disease_Prediction_KChanikya.pptx` | Project presentation |
| `README.md` | Project summary (this file) |

---

## 🚀 Future Work

- Integrate model into a Streamlit web app for real-time predictions
- Improve model with hyperparameter tuning or ensemble stacking
- Connect with EHR systems or wearable health devices for live use

---

## 👨‍💻 Author

**K. Chanikya**  

---

## 📌 License

This project is for educational and demonstration purposes only.
