# Airline_Passenger_Analysis
Machine Learning project analyzing airline passenger satisfaction with data preprocessing, EDA, and predictive modeling

# ✈️ Airline Passenger Satisfaction Analysis

## 📌 Project Overview
This project analyzes and predicts airline passenger satisfaction using survey and operational data.  
The workflow covers **data cleaning, exploratory data analysis (EDA), feature engineering, model building, hyperparameter tuning, and evaluation** with a focus on deploying a reliable machine learning model.

---

## 📊 Dataset
The dataset (`Airline.csv`) contains passenger survey responses and operational details.

- **Demographics**: `Gender`, `Customer Type`, `Type of Travel`, `Class`  
- **Service Ratings** (scale 1–5): `Inflight wifi service`, `Seat comfort`, `Food and drink`, `Cleanliness`, etc.  
- **Operational Metrics**: `Flight Distance`, `Departure/Arrival Delay in Minutes`  
- **Target Variable**: `satisfaction` (Satisfied / Neutral or Dissatisfied)

---

## ⚙️ Steps in the Project

### 1. Data Cleaning & Preparation
- Removed identifiers (e.g., `id`)  
- Handled missing values (`Arrival Delay in Minutes`)  
- Dropped highly correlated features to avoid leakage  
- One-hot encoded categorical variables  
- Label encoded target variable for compatibility with ML models  

### 2. Exploratory Data Analysis (EDA)
- Passenger demographics distribution  
- Travel type & class trends  
- Correlation heatmaps for feature relationships  
- Barplots & histograms for service ratings and satisfaction  

### 3. Model Building
- **Baseline Model**: Decision Tree with validation curves  
- **Final Model**: XGBoost Classifier with GridSearchCV  
- Hyperparameters tuned:  
  - `n_estimators`, `max_depth`, `learning_rate`, `subsample`, `colsample_bytree`  

### 4. Model Evaluation
- **Accuracy Score**  
- **Confusion Matrix**  
- **Classification Report (Precision, Recall, F1-Score)**  

---

## 🔑 Key Insights
- **Service quality** (inflight wifi, cleanliness, legroom) strongly impacts passenger satisfaction.  
- **Operational delays** have a moderate effect on dissatisfaction.  
- **XGBoost** effectively models non-linear interactions, achieving strong predictive performance.  

---

## 🛠️ Tech Stack
- **Programming**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost  
- **Tools**: Jupyter Notebook  


   git clone https://github.com/your-username/Airline_Passenger_Analysis.git
   cd Airline_Passenger_Analysis
