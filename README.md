# Stress-Level-Prediction Based on Digital Habits

This project aims to **predict stress levels** in individuals based on their digital habits using an end-to-end machine learning pipeline. It incorporates **data preprocessing**, **exploratory data analysis (EDA)**, **feature engineering**, and **model building** with **LightGBM**.

---

## Dataset Overview

- **Source:** `digital_habits_vs_mental_health.csv`
- **Features Include:**
  - Screen Time (Hours)
  - Sleep Hours
  - Study Hours
  - Social Media Usage
  - Online Class Time
  - Physical Activity Time
- **Target Variable:** Stress Level (categorized as `Low`, `Medium`, `High`)

---

## Project Workflow

1. **Data Import & Exploration**
   - Checked data types, null values, and distributions.
2. **EDA**
   - Correlation heatmaps
   - Distribution and boxplots for numeric features
   - Target class balance
3. **Data Cleaning & Feature Engineering**
   - Converted categorical labels
   - Label encoding
   - Removed mood-related columns to prevent **target leakage**
4. **Modeling with LightGBM**
   - Trained a LightGBM classifier
   - Tuned hyperparameters
   - Performed cross-validation
5. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - Confusion Matrix
6. **Insights**
   - Identified key features influencing stress levels
   - Evaluated model interpretability using feature importance

---

## Technologies Used

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-learn**
- **LightGBM**

---

## Key Results

- Best-performing model: **LightGBM Classifier**
- High accuracy in multi-class classification (Low/Medium/High stress)
- Clear correlation found between screen time, sleep, and stress

---

## Visuals & Interpretability

- Heatmaps for feature correlation
- Feature importance plot from LightGBM
- Confusion matrix heatmap

---

## Learnings

- Impact of digital lifestyle on mental health
- Importance of avoiding target leakage
- Practical experience with LGBM and evaluation strategies

---

## Future Scope

- Add real-time data collection via mobile apps or browser plugins
- Deploy as an interactive web app (e.g., with Streamlit or Flask)
- Experiment with deep learning models for higher accuracy
