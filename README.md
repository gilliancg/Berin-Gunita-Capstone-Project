# Berin & Gunita - Capstone Project

## Lifestyle and Learning – Predicting Student Performance

A capstone project that explores the impact of students' lifestyle habits on academic performance using machine learning.

## Authors

- Gillian C. Gunita  
- Farah Louise A. Berin  

## Project Overview

This project investigates how daily lifestyle choices—such as study hours, screen time, wellness habits, and mental health—affect students' final exam scores.  
By applying data analysis, clustering, and machine learning models, we aim to **predict performance outcomes** and identify meaningful behavior patterns among students.

## Dataset

The dataset contains 1,000 student records with features such as:

- `study_hours_per_day`  
- `social_media_hours`, `netflix_hours`  
- `sleep_hours`, `diet_quality`, `exercise_frequency`  
- `attendance_percentage`, `mental_health_rating`  
- `internet_quality`, `parental_education_level`, `part_time_job`  
- `extracurricular_participation`  
- `exam_score` (target variable)

## Methods & Techniques Used

### Data Preprocessing
- Missing value imputation
- Label encoding for categorical variables
- Feature scaling using StandardScaler
- **Feature engineering**:
  - `total_screen_leisure_hours` = social_media_hours + netflix_hours
  - `wellness_index` = average of diet quality, exercise frequency, and normalized sleep

### Exploratory Data Analysis (EDA)
- Histograms, scatter plots, box plots
- Correlation heatmap
- Key lifestyle patterns related to exam performance

### Clustering (Unsupervised Learning)
- K-Means clustering (using engineered lifestyle features)
- Elbow method and Silhouette score to determine optimal `k`
- Cluster profiling based on performance and behavior

### Regression (Supervised Learning)
- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- Evaluation: MAE, RMSE, R², cross-validation

### Classification (Optional)
- Converted `exam_score` into performance levels: **Low**, **Average**, **High**
- Trained classifiers:
  - Logistic Regression
  - Decision Tree
  - Random Forest
- Evaluation: Accuracy, F1-score, confusion matrix

## Key Findings

- **Higher study hours and wellness scores** correlate with better academic performance.
- **Increased leisure screen time** is linked to lower scores.
- **Cluster analysis** revealed distinct behavior groups with significant score differences.
- **Random Forest models** performed best in both regression and classification tasks.

## Recommendations

- Promote balanced screen time and consistent study routines.
- Support student wellness through health and mental well-being programs.
- Use predictive models to identify and assist students at risk of underperforming.
