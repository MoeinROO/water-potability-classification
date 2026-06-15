![Water Potability Banner](./images/image_gen_269f9392-6188-4707-aed6-99847900d04e_0.png)
# water-potability-classification
Predicting water potability using Random Forest &amp; XGBoost. Features advanced preprocessing with KNNImputer and Threshold Optimization.

Water Potability Prediction using ML
This project focuses on classifying water samples as Potable (1) or Non-Potable (0) based on their chemical and physical properties. It involves a complete data science pipeline: from EDA and missing value imputation to advanced machine learning modeling and hyperparameter tuning.

🧐 Problem Statement
Access to safe drinking water is essential for health. This project uses a dataset (from Kaggle) containing water quality metrics for 3,276 water bodies. The goal is to build a robust model to predict potability.

🛠 Tech Stack
Language: Python
Libraries: Pandas, NumPy, Scikit-Learn, XGBoost, Seaborn, Matplotlib
🚀 Key Features & Workflow
1. Exploratory Data Analysis (EDA)
Data Inspection: Analyzed data dimensions, types, and missing values.
Visualization: Used Scatter Plots (Hardness vs. Solids) and Correlation Matrices to find patterns.
Class Balance: Evaluated the potability distribution (Balanced/Imbalanced analysis).

3. Advanced Preprocessing
Handling Missing Values: Instead of simple mean-imputation, I used KNNImputer (n_neighbors=5) for more accurate data recovery.
Normalization: Applied StandardScaler to normalize features.
Distribution Analysis: Used KDE Plots to compare feature distributions (specifically Sulfate) before and after imputation.

4. Machine Learning Modeling
I implemented and compared two powerful ensemble models:
Random Forest Classifier
XGBoost Classifier

5. Optimization & Fine-tuning
Class Balancing: Addressed data imbalance to ensure the model doesn’t favor the majority class.
Hyperparameter Tuning: Used GridSearchCV to find the optimal parameters for both models.
Threshold Adjustment: Fine-tuned the decision threshold to minimize the probability of classifying unsafe water as potable (Safety First!).

📊 Results
Random Forest Accuracy: 0.6646341463414634
XGBoost Accuracy: 0.6310975609756098
Detailed Confusion Matrix and Classification Reports are available in the notebook.

📁 Project Structure
notebooks/: Contains the Jupyter Notebook with step-by-step implementation.
data/: The dataset used for training.
Created by Moein Roshan
