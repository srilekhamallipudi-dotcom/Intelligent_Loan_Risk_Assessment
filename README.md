🏦 Intelligent Loan Risk Assessment System using Machine Learning

📌 Project Overview

The Intelligent Loan Risk Assessment System is a machine learning-based application that predicts the risk level of loan applicants. It analyzes applicant details such as income, loan amount, interest rate, loan grade, employment length, and credit history to classify applicants into Low Risk and High Risk categories.

The system uses a trained Random Forest model and provides an interactive interface built with Streamlit.

🎯 Objectives

- Predict the risk level of loan applicants.
- Apply data preprocessing techniques to improve data quality.
- Handle class imbalance using SMOTE.
- Compare different machine learning algorithms.
- Evaluate model performance using standard evaluation metrics.
- Provide an interactive loan risk assessment interface.

📂 Dataset Description

The project uses a credit risk dataset containing applicant information and loan details.

Original dataset dimensions: 32,581 rows × 12 columns.

Important features include:

- Person Age
- Person Income
- Person Employment Length
- Loan Amount
- Loan Interest Rate
- Loan Grade
- Loan Intent
- Home Ownership
- Credit History Length
- Previous Default Information

Target variable: "loan_status"

⚙️ Methodology

1. Data Collection: Load the credit risk dataset.
2. Data Cleaning: Handle missing values and remove duplicate records.
3. Outlier Handling: Use the Interquartile Range (IQR) method and clipping.
4. Categorical Encoding: Convert categorical features into numerical values using ordinal mapping and one-hot encoding.
5. Feature Scaling: Apply StandardScaler to numerical model inputs.
6. Class Balancing: Apply SMOTE to the training data.
7. Model Training: Train Logistic Regression, Random Forest, and XGBoost models.
8. Model Evaluation: Compare models using accuracy, precision, recall, F1-score, and confusion matrices.
9. Prediction: Use the trained Random Forest model in the Streamlit application.

🤖 Machine Learning Algorithms

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

The deployed application uses the Random Forest Classifier for loan risk prediction.

📊 Model Performance

Recorded evaluation results:

Metric| Random Forest
Accuracy| 93.08%
Precision| 93.45%
Recall| 73.48%
F1-score| 82.27%

These results are from the project's recorded evaluation. Actual performance may vary with data and configuration.

✨ Key Features

- Loan applicant risk prediction
- Low Risk and High Risk classification
- Interactive Streamlit dashboard
- Model performance visualization
- Feature importance analysis
- What-If Risk Simulator to explore how changing applicant details affects predictions

🛠️ Technologies Used

- Programming Language: Python
- Data Processing: Pandas, NumPy
- Machine Learning: Scikit-learn, Imbalanced-learn, XGBoost
- Visualization: Matplotlib, Seaborn
- Web Application: Streamlit
- Model Storage: Joblib
- Version Control: Git and GitHub

📁 Project Files

- "app.py" – Streamlit application
- "random_forest_model.pkl" – Trained Random Forest model
- "scaler.pkl" – Saved feature scaler
- "rf_evaluation.pkl" – Saved model evaluation data, if included
- "credit_risk_dataset.csv" – Dataset, if included
- "requirements.txt" – Python dependencies
- "README.md" – Project documentation

🚀 How to Run the Project

1. Clone the Repository

git clone https://github.com/srilekhamallipudi-dotcom/Intelligent_Loan_Risk_Assessment.git
cd Intelligent_Loan_Risk_Assessment

2. Install Dependencies

pip install -r requirements.txt

3. Run the Application

streamlit run app.py

Open the local URL displayed in the terminal to access the application.

Note: The trained model, scaler, and any evaluation files required by "app.py" must be present at the paths expected by the code.

🔮 Future Enhancements

- Integrate real-time financial data.
- Improve model performance through hyperparameter tuning.
- Add explainable AI techniques for clearer predictions.
- Deploy the application to a cloud platform.
- Enhance security and data privacy.

⚠️ Disclaimer

This project is developed for educational and demonstration purposes. Predictions are model-based estimates and should not be used as the sole basis for actual loan approval decisions.

👩‍💻 Project Team

- M. Srilekha – 24B11AI236
- K. Navya Sri – 24B11AI182
- D. Thriveni – 24B11AI080

Project Guide: Mrs. P. Venkata Bala Annapurna

📜 License

This project is intended for educational purposes. Add a suitable open-source license if you intend to distribute it for reuse.
