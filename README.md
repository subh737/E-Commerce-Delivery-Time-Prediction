📝 Project Workflow

1️⃣ Data Exploration & Cleaning
Loaded dataset with 11K+ records and 12 features.
Performed Exploratory Data Analysis (EDA) using Matplotlib & Seaborn.
Checked distributions, correlations, and categorical/ordinal relationships.
Removed outliers using the IQR method.

2️⃣ Feature Engineering & Preprocessing
Encoded categorical variables using Ordinal Encoding.
Scaled numerical features using StandardScaler.
Created polynomial features (degree 2) to capture feature interactions.

3️⃣ Model Training
Split data into train, validation, and test sets (stratified by target).
Trained multiple models:
Logistic Regression
Random Forest
Gradient Boosting
XGBoost
CatBoost
Performed hyperparameter tuning using GridSearchCV for optimal parameters.
Saved the best models using Joblib.

4️⃣ Model Evaluation
Evaluated models on the test set using:
Accuracy, Precision, Recall, F1-score, AUC-ROC
Observed trade-offs between precision and recall:
Tree-based models (XGBoost, CatBoost, RF) → high precision, low recall.
Logistic Regression → better recall, moderate accuracy.

Key Insights:
Best accuracy: Gradient Boosting (61.7%)
Best AUC-ROC: CatBoost (0.644)
Logistic Regression has better recall → catches more delayed deliveries.
Overall performance shows moderate predictive capability, indicating scope for feature engineering and handling class imbalance.
