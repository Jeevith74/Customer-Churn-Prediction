# 📉 Customer Churn Prediction

### 📌 Project Overview

This project aims to predict whether a customer will churn (stop using a service) based on various customer attributes. It utilizes machine learning techniques to analyze historical data and build a predictive model. The project includes a complete pipeline from data preprocessing and feature engineering to model training and deployment/inference.

### 📑 Table of Contents

Project Overview

File Structure

Getting Started

Usage

Model Details

Contributing

### 📂 File Structure

The project repository is organized as follows:

### 📓 Notebooks

File Name

Description

CustomerChurnUpdated.ipynb

The main notebook containing the end-to-end workflow: EDA, Data Cleaning, Feature Selection, and Model Training.

app.ipynb

The inference interface. Use this notebook to load the saved model and make predictions on new customer data.

### 🤖 Models & Artifacts (.pkl files)

These serialized files are generated during training and are required for making predictions:

log_reg_model.pkl - Trained Logistic Regression model.

model.pkl - (Alternative) Additional trained model file.

scaler.pkl - Fitted scaler (Standard/MinMax) for normalizing numerical input.

label_encoder.pkl - Decodes the target variable (Churn/No Churn).

ordinal_encoder.pkl - Encodes ordinal categorical features.

final_columns.pkl - List of feature names to ensure input data matches the model structure.

### 🚀 Getting Started

Prerequisites

Ensure you have Python 3.x installed along with the following libraries:

pandas

numpy

scikit-learn

matplotlib

seaborn

jupyter

### Installation

#### Clone the repository:

git clone [https://github.com/yourusername/customer-churn-prediction.git](https://github.com/yourusername/customer-churn-prediction.git)
cd customer-churn-prediction


#### Install dependencies:

pip install pandas numpy scikit-learn matplotlib seaborn jupyter


### 💻 Usage

#### 1️⃣ Training the Model

To retrain the model or explore the data analysis process:

Open CustomerChurnUpdated.ipynb.

Run all cells sequentially.

This will process the dataset and overwrite the existing .pkl files in your directory.

#### 2️⃣ Making Predictions (Inference)

To predict churn for new customers:

Open app.ipynb.

Ensure all .pkl files are in the same directory.

Run the notebook cells to load the model and encoders.

Input your data when prompted (or modify the input cell) to see the prediction results.

## 📊 Model Details

Algorithm: Logistic Regression

Evaluation Metric: Accuracy, Precision, Recall, F1-Score (refer to the main notebook for charts).

Data Processing:

Categorical Encoding: Label Encoding & Ordinal Encoding.

Scaling: Numerical features are standardized.

### 🤝 Contributing

Contributions are welcome! Please follow these steps:

Fork the project.

Create your feature branch (git checkout -b feature/NewFeature).

Commit your changes (git commit -m 'Add some NewFeature').

Push to the branch (git push origin feature/NewFeature).

Open a Pull Request.

### 📝 License

This project is open-source and available for use under the MIT License.
