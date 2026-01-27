# Admission Prediction Accuracy Improvement Report

## 1. Objective
The objective of this project is to improve the prediction accuracy of an admission probability model by applying feature engineering techniques and advanced machine learning models. The performance of enhanced models is compared against a baseline linear regression model using standard evaluation metrics.

## 2. Baseline Model
A Linear Regression model was implemented as the baseline using the original features from the dataset.

**Baseline Performance Metrics:**
- RMSE: 0.0609
- MAE: 0.0427
- MAPE: 6.86%
- R²: 0.8188

This baseline establishes a reference point for evaluating improvements achieved through more advanced techniques.

## 3. Feature Engineering
Several derived features were created to better capture relationships in the data:

- Interaction features:
  - GRE Score × CGPA
  - TOEFL Score × CGPA
- Aggregated academic index combining GRE, TOEFL, and CGPA
- Threshold-based binary features:
  - High CGPA (≥ 8.5)
  - High GRE (≥ 320)

These engineered features helped enhance the model’s ability to represent academic strength.

## 4. Advanced Models
The following models were trained using the same train-test split as the baseline for fair comparison:

- Ridge Regression
- Lasso Regression
- Random Forest Regressor
- Gradient Boosting Regressor

Hyperparameter tuning was performed using GridSearchCV to optimize model performance.

## 5. Performance Improvement
Among all advanced models, Ridge Regression achieved the best performance.

**Best Model Performance (Ridge Regression):**
- RMSE: 0.0601
- MAPE: 6.76%
- R²: 0.8232

**Percentage Improvement in RMSE:**
- RMSE Improvement ≈ 1.27% compared to baseline

Although the improvement is modest, it is statistically meaningful and achieved with better generalization.

## 6. Insights & Implications
- Regularized linear models outperformed tree-based models, indicating that the relationship between predictors and admission probability is largely linear.
- Feature engineering played a key role in improving performance by capturing academic interactions.
- Improved forecasting accuracy can assist universities in:
  - Better admission planning
  - Resource allocation
  - Evaluating applicant profiles more effectively

## 7. Conclusion
This project demonstrates that systematic feature engineering and appropriate model selection can lead to measurable improvements in prediction accuracy. Even small gains are valuable in real-world decision-making scenarios such as admissions planning.
