# project-08

# Wine Quality Analysis and Machine Learning

## Project Overview

This project analyzes the Red Wine Quality and White Wine Quality datasets to explore the factors influencing wine quality using exploratory data analysis (EDA), machine learning, and clustering techniques.

The objectives of this project are to:

- Explore the chemical characteristics of wines.
- Identify the factors affecting wine quality.
- Predict wine quality scores using regression models.
- Classify high-quality wines.
- Classify red and white wines based on chemical properties.
- Segment wines into different groups using clustering.

---

## Dataset

The project combines two datasets:

- winequality-red.csv
- winequality-white.csv

After merging the datasets:

- Original observations: **6,497**
- After removing duplicate records: **5,320**
- Features: **11 physicochemical variables**
- Target variables:
  - Quality Score
  - Wine Type (Red / White)

Main features include:

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol

---

## Project Workflow

### 1. Data Preparation

- Imported and merged the red and white wine datasets.
- Added a Wine Type feature.
- Removed duplicate records.
- Checked missing values and data types.

### 2. Exploratory Data Analysis (EDA)

Performed exploratory analysis including:

- Wine Type Distribution
- Wine Quality Distribution
- Quality Distribution by Wine Type
- Correlation Analysis
- Alcohol vs. Wine Quality
- Alcohol Distribution by Wine Quality
- PCA Visualization

---

## Research Questions

### Research Question 1

**Can chemical properties predict wine quality?**

Model:

- Random Forest Regressor

Evaluation Metrics:

- MAE
- RMSE
- R² Score

---

### Research Question 2

**Can high-quality wines be identified using chemical properties?**

High-quality wines were defined as:

Quality ≥ 7

Model:

- Random Forest Classifier

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC AUC

---

### Research Question 3

**Can red and white wines be distinguished using chemical properties?**

Model:

- Random Forest Classifier

Evaluation Metrics:

- Accuracy
- ROC AUC
- Confusion Matrix

---

### Research Question 4

**Can wines be segmented into different chemical profiles?**

Model:

- K-Means Clustering

Visualization:

- PCA Projection
- Cluster Summary

---

## Machine Learning Models

Regression

- Random Forest Regressor

Classification

- Random Forest Classifier (High-Quality Wine)
- Random Forest Classifier (Wine Type)

Clustering

- K-Means
- PCA Visualization

---

## Key Findings

- Alcohol is the strongest predictor of wine quality.
- Density and volatile acidity are negatively associated with wine quality.
- Random Forest achieved good performance in predicting wine quality.
- High-quality wines can be classified with strong predictive performance.
- Red and white wines can be distinguished almost perfectly using chemical properties.
- K-Means identified four meaningful wine segments with different chemical characteristics.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## Project Structure

```
Wine Quality Project/
│
├── winequality-red.csv
├── winequality-white.csv
├── Wine_Quality_Analysis.qmd
├── README.md

```


---

## Final Conclusion

This project demonstrates how machine learning techniques can effectively analyze wine quality using physicochemical properties. By combining exploratory data analysis, regression, classification, and clustering, the project provides meaningful insights into the factors influencing wine quality, accurately distinguishes wine types, and identifies distinct wine segments. These findings can support quality assessment, product segmentation, and decision-making within the wine industry.