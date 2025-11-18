## PCOS Prediction Model

Polycystic Ovary Syndrome (PCOS) is one of the most common endocrine disorders affecting women of reproductive age.
In Pakistan, its prevalence is around 52%, significantly higher than many Western populations. Early awareness and screening are therefore essential.

This project is a PCOS Test Package for Women, built to raise awareness and allow users to review the Random Forest model used for prediction.

⚠️ Note: This project is for educational and awareness purposes only and not for medical diagnosis.

📌 Project Overview

This repository contains:

A Jupyter Notebook (pcospredictor.ipynb) implementing a Random Forest classifier with GridSearchCV and Stratified K-Folds
A model file PCOSpredictor.pkl

Preprocessing, feature selection, and model evaluation
Prediction probabilities for Healthy vs. High-Risk women
Integration into a web app UI: [PCOS Predictor App](https://pcos-predictor-eight.vercel.app/)

📂 Dataset

The dataset comes from Kaggle:
[🔗 PCOS Dataset](https://www.kaggle.com/datasets/sahilkoli04/pcos2023)

🧠 Model Details

Algorithm: Random Forest Classifier
Hyperparameter Tuning: GridSearchCV on Stratified K-Folds
Best Parameters:

{
    'max_depth': 10,
    'min_samples_leaf': 2,
    'min_samples_split': 5,
    'n_estimators': 200
}


Performance Metrics:

Metric	Value
Accuracy	0.946
Precision 0	0.95
Recall 0	0.99
F1-Score 0	0.97
Precision 1	0.90
Recall 1	0.69
F1-Score 1	0.78
Macro Avg	0.88
Weighted Avg	0.94

Interpretation:

Healthy women have a predicted risk of ~2.09%

High-risk women have a predicted risk of ~92.77%

🔑 Features Used
features = [
    'Age', 'Weight', 'Height', 'BloodGroup', 'PeriodFrequency', 
    'GainedWeight', 'ExcessiveHair', 'DarkSkin', 'Hair Loss', 
    'FaceAcne', 'FastFood', 'RegularExercise', 'MoodSwings', 
    'RegularPeriods', 'PeriodDuration', 'BMI'
]

Users can enter their details and receive PCOS risk percentages for educational purposes.

📄 Repository Structure
PCOSPredictionModel/
│
├── pcospredictor.ipynb # Random Forest model & analysis
├── PCOSpredtictor.pkl                # saved model
├── README.md                # Project documentation
└── (Dataset via Kaggle link)

💡 Purpose of the Project

Raise awareness about PCOS prevalence in Pakistan

Provide an educational example of medical ML modeling

Allow review of model performance and feature importance

Promote early detection and lifestyle awareness

Reminder: This is not a diagnostic tool. Always consult a doctor for medical concerns.

🤝 Contributions

Contributions, feedback, or improvements are welcome! Submit issues or pull requests on GitHub.
