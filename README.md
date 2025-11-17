# 🩺 Diabetes Prediction using Machine Learning

This project analyzes the Pima Indians Diabetes dataset to predict the likelihood of diabetes using multiple machine learning models. The goal is to demonstrate a complete and reproducible workflow from data exploration to model evaluation and interpretation.

## 📘 Project Overview

The notebook covers the following steps

1. Exploring the dataset and understanding key features  
2. Checking data quality, distributions and correlations  
3. Preparing the data through scaling and splitting  
4. Training classification models including Decision Tree, Logistic Regression, SVM, Naive Bayes and Random Forest  
5. Evaluating the models using accuracy, precision, recall and F1 score  
6. Comparing results and identifying the most effective model  

## 📊 Dataset Information

The dataset contains 768 samples with 9 medical features such as glucose level, BMI, age and blood pressure.  
The target variable indicates whether the patient is diabetic or not.  
The dataset is available from the UCI Machine Learning Repository.

## 🤖 Models Trained

The following models were implemented and evaluated

- Decision Tree Classifier  
- Logistic Regression  
- Support Vector Machine  
- Naive Bayes  
- Random Forest Classifier  

Each model was trained on standardized data and evaluated using the same test set.

## 🏆 Key Results

Naive Bayes provided the strongest performance among all models.  
It achieved the highest accuracy of **0.766** and the highest recall of **0.709**.  
This means it correctly identified more diabetic cases compared to the others,  
which is important for screening where missing positive cases should be minimized.

### 📈 Model Comparison Table

| Model              | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|-----------|--------|----------|
| Decision Tree       | 0.746    | 0.826     | 0.727  | 0.672    |
| Logistic Regression | 0.753    | 0.649     | 0.672  | 0.660    |
| SVM                 | 0.727    | 0.632     | 0.563  | 0.596    |
| Naive Bayes         | 0.766    | 0.661     | 0.709  | 0.684    |
| Random Forest       | 0.727    | 0.618     | 0.618  | 0.618    |

## 🎯 Final Conclusion

Naive Bayes is the most effective model for this dataset.  
Its strong recall and balanced scores make it a reliable option for early detection of diabetes.  
Logistic Regression and Random Forest also performed consistently, while Decision Tree and SVM produced moderate results.

## 🚀 Next Steps

Future work can include

- Hyperparameter tuning to improve model performance  
- Feature engineering or selection to reduce noise  
- Applying resampling methods such as SMOTE to improve recall  
- Trying advanced models such as Gradient Boosting or XGBoost  
- Deploying the final model with Streamlit for an interactive interface  

## 📦 Installation

To set up the environment and install all required packages, follow the instructions below based on your operating system.
```
# Clone repository
git clone <repository-url>

# macOS

Open Terminal and run

pip install -r requirements.txt

# Windows

Open Command Prompt or PowerShell and run

pip install -r requirements.txt


# Linux

Open Terminal and run

pip install -r requirements.txt

```

## 📁 Repository Structure
```
.
├─ data
│  └─ diabetes.csv
├─ notebooks
│  └─ Diabetes_Prediction.ipynb
├─ requirements.txt
├─ .gitignore
└─ README.md
```