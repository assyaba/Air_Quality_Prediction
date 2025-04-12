# Air_Quality_Prediction
 
# Pollution Data Analysis & Modeling

This repository contains an R-based data analysis pipeline for exploring and modeling pollution-related data using the `updated_pollution_dataset.csv` dataset. The project includes data preprocessing, exploratory data analysis (EDA), and several statistical modeling techniques.

---

## 🎓 Project Background: MSBA Capstone – Predicting Air Quality Level

This project was conducted as part of a graduate course at the Raymond A. Mason School of Business (William & Mary) by Group 6 – Assya Ba, Ben Greenberg, Stefan Ngoh, Elaina Longjohn.

### 🧭 Objective

To uncover the key factors influencing air pollution and develop predictive models that accurately classify air quality levels based on pollutant, geographic, and climatic data.

### 🧪 Data Source

- Source: Kaggle ([Link](https://www.kaggle.com/datasets/muhammadtalha07/air-quality-and-pollution-assessment))
- Features: PM2.5, PM10, NO2, SO2, CO, temperature, humidity, population, proximity to industrial areas.
- Target Variable: Air quality classified into 4 levels — **Good**, **Moderate**, **Poor**, and **Hazardous**.

---

## 🔍 Approach

Several predictive modeling techniques were tested to classify air quality:

- **Logistic Regression (Binary)**: Simplified the problem to “Acceptable” vs “Unacceptable.”
- **K-Nearest Neighbors (KNN)**: Used as a baseline; struggled with poor/hazardous class prediction.
- **Linear Discriminant Analysis (LDA)**: Best-performing model, with 93.55% accuracy and 98.25% sensitivity when classifying into all 4 categories.

---

## 📊 Results & Insights

- **LDA** was the most accurate model for 4-class classification.
- **Grouped logistic regression** yielded 96.70% accuracy.
- **KNN** showed weaker performance on edge cases.
- Proximity to industrial areas and pollutants like PM2.5 and NO2 had strong predictive power.

---

## 🌍 Implications

- These models can help policymakers assess and respond to urban air quality concerns.
- Highlights importance of urban planning: residential zones should be distanced from industrial areas.
- Suggests promoting green infrastructure and urban greening to reduce pollution impact.

---

## 📦 Requirements

Install the following R packages:

```r
install.packages(c(
  "ISLR2", "lmtest", "mltools", "ggplot2", "tidyverse", "rattle",
  "MASS", "caret", "car", "summarytools", "corrplot", "mlbench"
))
```

---

## 📁 Files

- `notebook.ipynb`: The core analysis notebook.
- `updated_pollution_dataset.csv`: Dataset file (ensure it's in the same directory when running the notebook).

---

## ▶️ How to Run

1. Open the `notebook.ipynb` file in an R-compatible Jupyter environment.
2. Run the cells step-by-step to perform the analysis.
3. Ensure the dataset CSV is present in the working directory.

---

## 📚 References

- Dataset: [Kaggle - Air Quality and Pollution Assessment](https://www.kaggle.com/datasets/muhammadtalha07/air-quality-and-pollution-assessment)

---

## 🙌 Acknowledgements

Thank you to Frank Wood and Monica Tremblay for their mentorship and guidance throughout the project.
