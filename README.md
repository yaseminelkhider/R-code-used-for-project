# Statistical Analysis of Key Health Indicators Predicting Diabetes 🩺📊


## 📌 Project Overview

This project demonstrates statistical analysis techniques used to explore which health indicators are most predictive of diabetes. We conducted a comprehensive study involving exploratory data analysis, hypothesis testing, regression modeling, and both parametric and non-parametric methods.

➡️ **R Code**: [View on GitHub](https://github.com/yaseminelkhider/R-code-used-for-project/blob/main/main%20code)

---

## 🧠 Abstract

Our study identifies blood glucose and HbA1c levels as the most predictive indicators of diabetes. Age also plays a role, but BMI shows only weak predictive power. These findings emphasize the importance of blood sugar control in assessing diabetes risk.

---

## 🔍 Table of Contents

1. [Introduction](#introduction)
2. [Data Acquisition & Exploration](#data-acquisition--exploration)
3. [Descriptive Statistics & Distribution Analysis](#descriptive-statistics--distribution-analysis)
4. [Central Tendency & Variation](#central-tendency--variation)
5. [Normality Testing](#normality-testing)
6. [Confidence Intervals](#confidence-intervals)
7. [Inferential Hypothesis Testing](#inferential-hypothesis-testing)
8. [Mean, Proportion, and Variance Tests](#mean-proportion-and-variance-tests)
9. [Predictive Modeling & Regression](#predictive-modeling--regression)
10. [Goodness-of-Fit & Association Tests](#goodness-of-fit--association-tests)
11. [ANOVA Analysis](#anova-analysis)
12. [Non-Parametric Tests](#non-parametric-tests)
13. [Results & Interpretation](#results--interpretation)
14. [Conclusion](#conclusion)

---

## Introduction

We aimed to identify which factors (HbA1c, blood glucose, age, BMI) most strongly predict diabetes using a dataset of 100,000 individuals.

---

## Data Acquisition & Exploration

- 📍 Source: [Kaggle Diabetes Prediction Dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset)
- Includes: Age, blood pressure, hemoglobin, cholesterol, glucose, HbA1c, BMI, diabetes status

---

## Descriptive Statistics & Distribution Analysis

We performed:
- Frequency distribution
- Histograms and boxplots
- Class widths, limits, and boundaries

**Key Distributions:**
- Blood glucose: multimodal & right-skewed
- HbA1c: unimodal & right-skewed
- Age: multimodal
- BMI: unimodal

---

## Central Tendency & Variation

- Mean age: 41.9, BMI: 27.3, Glucose: 138
- Highest variation seen in **glucose**
- Least variation in **HbA1c**

---

## Normality Testing

- ❌ Shapiro-Wilk & Q-Q plots show **no variable follows a normal distribution**
- ✅ Central Limit Theorem holds true for all sample means

---

## Confidence Intervals

**95% CI for Difference in Means (Diabetics vs Non-Diabetics):**
- Age: ~21 years older
- BMI: +5.1
- Glucose: +61.2 mg/dL
- HbA1c: +1.5%

---

## Inferential Hypothesis Testing

We used **logistic regression** for binary diabetes outcome:

| Predictor | Coefficient | Significance |
|-----------|-------------|--------------|
| HbA1c     | ✅ Strongest |
| Glucose   | ✅ Strong    |
| Age       | ✅ Moderate  |
| BMI       | ✅ Weak      |

---

## Mean, Proportion, and Variance Tests

- **Two Means**: All variables significantly different between groups
- **Two Proportions**: Hypertension 4.2x more common in diabetics
- **Two Variances**: Diabetics had more age variation, less glucose/BMI variation

---

## Predictive Modeling & Regression

- Logistic models + residual diagnostics
- **Pseudo R² Scores:**
  - HbA1c: 0.34 (McFadden)
  - Glucose: 0.26
  - Age: 0.13
  - BMI: 0.07

---

## Goodness-of-Fit & Association Tests

- ✅ Chi-square test: Diabetes is NOT evenly distributed
- ✅ Diabetes is significantly related to **hypertension** and **heart disease**
- ⚠️ Very weak link with gender

---

## ANOVA Analysis

### One-Way ANOVA:
All predictors (age, glucose, HbA1c, BMI) show significant mean differences between diabetic and non-diabetic groups.

### Two-Way ANOVA:
- HbA1c and Glucose: significantly affected by diabetes, not age
- BMI: affected by both diabetes, age, and their interaction

---

## Non-Parametric Tests

- **Mann-Whitney U Test**: All variables differ significantly
- **Spearman ρ**: Highest for HbA1c (ρ = 0.329)
- **Runs Test**: Glucose and HbA1c show non-random patterns with diabetes status

---

## Results & Interpretation

- **Top Predictors**: HbA1c and blood glucose levels
- Age matters, but doesn’t change the predictive strength of glucose markers
- BMI is significant but weak

---

## Conclusion

### 🔑 Key Takeaways:
- Blood sugar markers (HbA1c & Glucose) are the **most reliable predictors**
- Age and BMI contribute, but less significantly

### 🩺 Real-World Implications:
- Routine screening should prioritize HbA1c and Glucose
- Public health policies should target older and high-BMI populations

### 🔭 Future Work:
- Longitudinal tracking
- Include lifestyle & genetic data
- Apply machine learning for deeper insights

---

## 📚 References

- [Kaggle Diabetes Dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset)

---

## 🧪 Appendix: R Code

R code used for this analysis is available on GitHub:  
👉 [View R Code](https://github.com/yaseminelkhider/R-code-used-for-project/blob/main/main%20code)
