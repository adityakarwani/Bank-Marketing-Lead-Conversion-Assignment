# Bank Marketing Lead Conversion Analysis

## Setup Instructions
1. Clone this repository
2. Install requirements: `pip install -r requirements.txt`
3. Run the Jupyter notebook: `jupyter notebook bank_marketing.ipynb`

## Summary of Findings

### Key Insights
- The dataset shows significant class imbalance with only ~11% positive cases (term deposit subscriptions)
- Age and job type showed interesting relationships with subscription rates
- Duration of the call appears to be the most important predictive feature

### Model Performance
- **Logistic Regression (Baseline):**
  - Accuracy: 0.89, AUC-ROC: 0.78, F1: 0.39
- **Random Forest with SMOTE (Improved):**
  - Accuracy: 0.90, AUC-ROC: 0.93, F1: 0.47

### What Worked
- Addressing class imbalance with SMOTE improved recall of positive cases
- Random Forest outperformed Logistic Regression in all metrics
- Feature importance analysis provided actionable business insights

### Next Steps
- Experiment with other algorithms (XGBoost, Neural Networks)
- More sophisticated feature engineering (interaction terms)
- Deeper hyperparameter tuning
- Cost-sensitive learning to optimize business outcomes
