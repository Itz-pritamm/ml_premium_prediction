# ml_premium_prediction
🔍 Project Highlights:
Objective: Predict the insurance premium cost based on demographic and medical data.

Data Preparation:

Cleaned and handled null values effectively.

Transformed and formatted data for better model performance.

Extracted key insights from EDA to guide modeling decisions.

📊 Initial ML Model:
Applied machine learning on the overall dataset.

Achieved 98% accuracy, but faced high error variance (30% difference between actual and predicted values).

🧑‍⚕️ Age-Based Data Split:
Found a critical issue with the age feature during analysis.

Split the data into two groups:

Young group (age ≤ 25)

Rest group (age > 25)

🔄 Improved Modeling:
Trained separate ML models for each group:

Rest group: Achieved 99% accuracy.

Young group: Initially gave 60% accuracy.

Introduced a new feature: Genetic Risk Score (based on medical history).

Post-feature engineering, the young group model improved to 98% accuracy.

✅ Final Outcome:
Two specialized models:

model_young.joblib for age ≤ 25

model_rest.joblib for others

Significant accuracy improvement across all age groups.

Developed a scalable prediction pipeline ready for deployment.
