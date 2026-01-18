# 🛒 E-Commerce Purchase Prediction Using Machine Learning

## 📌 Project Overview
This project focuses on building a **machine learning model** to predict whether an online visitor is likely to make a purchase based on their **session-level behavior** on an e-commerce website.

The prediction helps businesses understand customer intent and improve decision-making related to marketing, personalization, and sales optimization.

---

## 🎯 Problem Statement
You are hired as a ML engineer to build a predictive model that can determine whether a visitor is likely to make a purchase based on their session behavior.

---

## 📂 Dataset Description
The dataset contains information about user interactions during an online session, including:

- Number of pages visited
- Time spent on different page types
- Bounce and exit rates
- Visitor type (new or returning)
- Weekend or weekday visits
- Month of visit

**Target Variable:**
- `Revenue`  
  - `1` → Purchase made  
  - `0` → No purchase  

---

## 🧠 Approach & Methodology

### 1️⃣ Exploratory Data Analysis (EDA)
- Analyzed distribution of numerical features
- Checked class imbalance in target variable
- Used visualizations such as:
  - Histograms
  - Box plots
  - Correlation heatmaps

### 2️⃣ Feature Engineering
Created meaningful features to improve model performance:
- `TotalPages`
- `TotalDuration`
- `EngagementScore`
- `ExitBounceDiff`
- `HighBounce` flag

### 3️⃣ Data Preprocessing
- Label Encoding for categorical features
- Binary encoding for boolean columns
- No feature scaling (Decision Trees do not require it)

### 4️⃣ Model Building
- Algorithm used: **Decision Tree Classifier**
- Hyperparameters tuned:
  - `max_depth`
  - `min_samples_leaf`
  - `class_weight = balanced`

### 5️⃣ Model Evaluation
- Evaluation Metric: **F1 Score**
- Reason: Dataset is imbalanced, and F1-score balances precision and recall
- Confusion Matrix used for performance analysis

---

## 📊 Results
- The model successfully predicts purchase intent with a balanced performance
- Feature importance analysis showed that:
  - PageValues
  - BounceRates
  - ProductRelated_Duration  
  are strong predictors of purchase behavior

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📁 Project Structure
├── E-commerse_purchase_prediction.ipynb
├── shop_smart_eccommerce.csv
├── README.md
