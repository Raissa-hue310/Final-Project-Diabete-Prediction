# Final-Project-Diabete-Prediction
The goal of this project is to develop a comprehensive AI application that uses machine learning models to solve a real-world problem. 

---

## 🎯 Project Objectives

1. **Define a real-world ML problem** (Diabetes prediction).  
2. **Load and preprocess a real dataset**.  
3. **Train and optimize a machine learning model**.  
4. **Evaluate model performance using multiple metrics**.  
5. **Analyze fairness across different age groups**.  
6. **Explain model predictions using SHAP & LIME**.  
7. **Deploy the model in Google Colab with an interactive function**.

---

## 📊 Dataset Description

**Dataset:** Pima Indians Diabetes Dataset  
**Source:** Kaggle / UCI Repository  
**Rows:** 768  
**Target Variable:** `Outcome`  
- `0` = No diabetes  
- `1` = Diabetes  

### Features
| Feature | Description |
|---------|-------------|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure |
| SkinThickness | Triceps skin fold thickness |
| Insulin | Serum insulin |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Genetic risk score |
| Age | Age in years |

---

## 🛠️ Tools and Libraries Used

- **Python**
- **Google Colab**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-Learn**
- **SHAP**
- **LIME**
- **Fairlearn**

---

## 🔧 Machine Learning Workflow

### 1️⃣ Data Preprocessing
- Handling invalid zero values  
- Median imputation  
- Scaling using StandardScaler  
- Exploratory Data Analysis (Heatmaps, Histograms, Boxplots)

### 2️⃣ Model Training
- Logistic Regression (baseline model)  
- Hyperparameter tuning using GridSearchCV  
- 5-fold cross validation  
- ROC-AUC scoring  

### 3️⃣ Model Evaluation
Metrics used:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  
- Confusion Matrix  
- ROC Curve  

### 4️⃣ Fairness Analysis
Using **Fairlearn**, performance was evaluated across **age groups**:
- Accuracy by group  
- Selection rate  
- False positive rate  

### 5️⃣ Explainability
- **SHAP Summary Plot** (global explanation)  
- **SHAP Force Plot** (local explanation)  
- **LIME Output** for individual predictions  

### 6️⃣ Deployment
A simple interactive Python function built in Colab:

- User inputs the 8 clinical features  
- Model returns:
  - **Prediction** (Diabetes / No Diabetes)
  - **Probability score**

---

pip install -r requirements.txt
python your_script.py
