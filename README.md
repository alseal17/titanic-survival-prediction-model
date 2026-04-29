# 🚢 Titanic Survival Prediction Model

## ⭐ Project Highlights

- Built a machine learning model to predict Titanic passenger survival  
- Implemented preprocessing pipelines to ensure consistent data handling and prevent data leakage  
- Performed feature engineering and categorical encoding  
- Compared multiple classification models using validation metrics  
- Generated predictions for Kaggle submission  

---

## 📌 Overview

This project uses the Titanic dataset to predict passenger survival based on demographic and travel-related features. The goal is to demonstrate a complete machine learning workflow, including data preprocessing, exploratory analysis, model training, evaluation, and prediction generation.

This project is based on the classic Titanic classification problem, where the target variable is whether a passenger survived.

---

## 🎯 Objectives

- Explore passenger survival patterns  
- Clean and preprocess missing or categorical data  
- Engineer useful features for model training  
- Train classification models to predict survival  
- Evaluate model performance  
- Generate predictions for submission  

---

## 📊 Dataset

The dataset comes from the Kaggle Titanic competition.

Features include:

- Passenger class  
- Sex  
- Age  
- Fare  
- Number of siblings/spouses aboard  
- Number of parents/children aboard  
- Embarkation port  
- Survival outcome  

The raw dataset is not included in this repository. It can be downloaded from Kaggle:

https://www.kaggle.com/competitions/titanic

---

## 📁 Project Structure

- notebooks/ → exploratory analysis and modeling workflow  
- data/ → raw and processed datasets (not included)  
- reports/ → figures and outputs  
- src/ → reusable code for future scalability  

---

## 🔍 Key Insights

- Female passengers had significantly higher survival rates than males  
- First-class passengers were more likely to survive than lower classes  
- Age showed moderate influence, with younger passengers having slightly higher survival rates  

---

## 🔧 Data Preparation & Feature Engineering

The dataset was cleaned and prepared for modeling through:

- Encoding categorical variables (e.g., sex, embarkation port, passenger class)  
- Handling missing values through preprocessing pipelines  
- Creating structured feature sets for consistent model training and evaluation  

Preprocessing was implemented using scikit-learn pipelines to ensure transformations were applied consistently across training and validation data, helping prevent data leakage.

---

## 🤖 Modeling Approach

Models were implemented using scikit-learn pipelines to ensure consistent preprocessing and reproducibility.

### Models Evaluated

- Logistic Regression  
- Random Forest  
- Gradient Boosting  

Model evaluation evolved from a basic train/test split approach to a more structured validation process, improving reliability of performance comparisons across models.

---

## 📈 Model Results

| Model | Cross-Validation Score | Validation Score |
|------|-------------------------|------------------|
| Logistic Regression | 0.8249 | 0.8212 |
| Random Forest | 0.8059 | 0.8436 |
| Gradient Boosting | 0.8429 | 0.8324 |

Gradient Boosting produced the strongest cross-validation performance, while Random Forest achieved the highest validation score.

---

## 🧠 Interpretation

The model results suggest that passenger survival was strongly influenced by demographic and travel-related factors, particularly sex and passenger class. Ensemble models performed well because they were able to capture nonlinear relationships between features.

Although the validation scores were promising, Kaggle public leaderboard scores were lower, highlighting the importance of generalization and the difference between local validation performance and unseen test data.

This project also demonstrates the importance of structured preprocessing and model evaluation workflows when working with real-world datasets.

---

## 🚀 Kaggle Submission

Predictions were generated for the Kaggle test dataset and exported as a submission file.

Best public Kaggle score observed:

0.76076

---

## ⚠️ Limitations

- Public leaderboard score may not fully reflect final model performance  
- Some missing values required imputation  
- Feature engineering could be expanded further  
- Dataset is relatively small and historically limited  

---

## 🔮 Future Improvements

- Tune model hyperparameters more extensively  
- Add more advanced feature engineering  
- Test additional models such as XGBoost or LightGBM  
- Use feature importance or SHAP values for interpretability  
- Improve validation strategy to better match Kaggle performance  

---

## 🛠 Tools & Technologies

- Python  
- Pandas / NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  
- Kaggle  
