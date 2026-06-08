# Customer Churn Prediction using Deep Learning

## Project Overview
This project predicts whether a customer is likely to leave a company (churn) using a Deep Learning model built with TensorFlow/Keras. The model analyzes customer demographic and account-related information to identify customers at risk of churning, helping businesses improve customer retention strategies.

## Features
- Data preprocessing and cleaning
- Feature encoding and scaling
- Artificial Neural Network (ANN) model
- Customer churn prediction
- Model evaluation and performance metrics
- Streamlit web application for real-time predictions

## Dataset
The dataset contains customer information such as:

- Customer ID
- Gender
- Age
- Tenure
- Balance
- Number of Products
- Credit Score
- Geography
- Estimated Salary
- Active Membership Status
- Churn Status (Target Variable)

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Streamlit
- Pickle


## Project Structure


Customer-Churn-Prediction/
│
├── data/
│ └── churn.csv
│
├── models/
│ ├── model.h5
│ ├── scaler.pkl
│ ├── label_encoder_gender.pkl
│ └── onehot_encoder_geo.pkl
│
├── app.py
├── train.py
├── prediction.py
├── requirements.txt
└── README.md


## Model Architecture
The ANN model consists of:

- Input Layer
- Hidden Layer 1 (ReLU Activation)
- Hidden Layer 2 (ReLU Activation)
- Output Layer (Sigmoid Activation)

Loss Function:
- Binary Crossentropy

Optimizer:
- Adam

Evaluation Metric:
- Accuracy

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd Customer-Churn-Prediction
Install Dependencies
pip install -r requirements.txt
Train the Model
python train.py

The trained model and preprocessing files will be saved in the models/ directory.

Run the Streamlit Application
streamlit run app.py

Open your browser and visit:

http://localhost:8501
Prediction Workflow
Enter customer details.
Data is preprocessed using saved encoders and scaler.
ANN model predicts churn probability.
Result is displayed as:
Customer Likely to Churn
Customer Likely to Stay
Results

The model achieves strong performance in predicting customer churn and can be used to identify high-risk customers for retention campaigns.

Future Improvements
Hyperparameter tuning
Feature engineering
Model explainability using SHAP
Deployment on Streamlit Cloud
Integration with business dashboards
Author

Deepak Singh
