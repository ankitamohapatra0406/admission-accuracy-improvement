# 🎓 Admission Prediction Accuracy Improvement 
## 📌Project Overview
This project focuses on improving the accuracy of predicting a student’s probability of admission using machine learning techniques. Starting from a baseline linear regression model, the project applies feature engineering, advanced regression models, and hyperparameter tuning to achieve measurable performance improvements.

The work follows a structured, reproducible ML workflow and emphasizes fair model comparison.

## 🎯Objective
- Build a baseline admission prediction model
- Improve prediction accuracy using feature engineering
- Train and tune advanced machine learning models
- Evaluate performance improvements using standard metrics
- Present insights through analysis and reporting

# 📊Dataset
- Source: Admission_Predict.csv (Graduate Admission dataset)
- Target Variable: Chance of Admit
- Key Features:
   - GRE Score
   - TOEFL Score
   - CGPA
   - University Rating
   - SOP & LOR Strength
   - Research Experience

## Results Summary
| Model             | RMSE   | MAPE (%) | R²     |
| ----------------- | ------ | -------- | ------ |
| Baseline (Linear) | 0.0609 | 6.86     | 0.8188 |
| Ridge Regression  | 0.0601 | 6.76     | 0.8232 |
| Lasso Regression  | 0.0611 | 6.88     | 0.8172 |
| Random Forest     | 0.0651 | 7.07     | 0.7927 |
| Gradient Boosting | 0.0650 | 7.26     | 0.7931 |

Best Model: Ridge Regression
RMSE Improvement: ~1.27%

# 💡Key Insights
- Regularized linear models performed better than tree-based models
- Feature engineering contributed more to performance gains than model complexity
- Admission probability shows strong linear relationships with academic metrics
- Small improvements in RMSE are meaningful in real-world admission decision systems
