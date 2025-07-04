# 🧠 Credit Risk Prediction using Machine Learning

This project builds a machine learning pipeline to assess the **creditworthiness** of loan applicants using the **German Credit dataset**. It includes preprocessing, model training using multiple classifiers, and explainability using **SHAP**. The project is also equipped with a Streamlit UI and FastAPI API backend — ready for real-world deployment.

---

## 📌 Project Highlights

- ✅ Model-based imputation for missing financial features
- 🔍 SHAP Explainability to interpret model predictions
- 📊 Tried and compared: Random Forest, XGBoost, LightGBM, CatBoost
- 📈 Feature importance visualization
- 🧠 Optimized preprocessing pipeline
- 🎯 Deployment-ready (Streamlit UI)

---

## 📁 Project Structure

### 🔹 Step 1: Data Preprocessing

We begin by cleaning and preparing the dataset:
- Missing values in `Saving accounts` and `Checking account` are filled using **model-based imputation**
- Categorical features like `Sex`, `Housing`, `Purpose` are label-encoded
- The target variable `Risk` is mapped (`good` → 0, `bad` → 1)
- Some skewed numeric features like `Credit amount` are log-transformed
- The data is split into training and test sets

✅ This step ensures the data is ML-ready and improves model performance.

---

### 🔹 Step 2: Model Training

We experiment with and compare 4 classifiers:
- **Random Forest**
- **XGBoost**
- **LightGBM**
- **CatBoost**

All models are trained with proper cross-validation and grid search.

We evaluate them using:
- Accuracy
- Precision / Recall
- Confusion Matrix

✅ These models predict the likelihood of a customer defaulting on a loan.

---

### 🔹 Step 3: SHAP Explainability

We use **SHAP (SHapley Additive Explanations)** to:
- Understand which features influence predictions the most
- Create global and individual explanation plots

📊 Key features:
- Credit amount
- Duration
- Saving accounts
- Checking account
- Purpose

✅ Helps stakeholders and regulators trust the model’s decisions.

---

### 🔹 Step 4: Streamlit UI

We built a user-friendly **Streamlit app**:

- Enter features like age, credit amount, savings, etc.
- Click **"Predict"**
- Get an instant prediction: **Good Credit** or **Bad Credit**

✅ Business users (loan officers) can interact with the model without writing any code.




