# 🚢 Titanic Survival Prediction (Kaggle)

## 📌 Project Overview
This project predicts whether a passenger survived the Titanic disaster using machine learning models.  
The dataset is provided by [Kaggle’s Titanic competition](https://www.kaggle.com/c/titanic), one of the most popular beginner ML challenges.  

I experimented with multiple ML algorithms, performed feature engineering, and tuned hyperparameters to achieve the best accuracy.  

---

## 📊 Dataset
- **Train.csv** – contains passenger details + survival labels  
- **Test.csv** – contains passenger details without labels (used for submission)  
- **Gender_submission.csv** – baseline sample submission  

Key features include: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`.  

---

## ⚙️ Approach
1. **Exploratory Data Analysis (EDA)** – Checked survival rates by sex, class, age distribution, etc.  
2. **Data Cleaning** – Handled missing values (`Age`, `Embarked`, `Fare`).  
3. **Feature Engineering**  
   - Created new features (`FamilySize`, `IsAlone`, `Title` from Name).  
   - Converted categorical variables (`Sex`, `Embarked`, `Title`) into numerical.  
4. **Model Training**  
   - Tested multiple algorithms:  
     - Logistic Regression  
     - Random Forest  
     - Support Vector Machine (SVM)
     - Guassian Naive Bayes   
     - K-Nearest Neighbors (KNN)  
     - XGBoost  
   - Tuned hyperparameters using GridSearchCV.  
5. **Model Selection** – Chose the best-performing model based on cross-validation accuracy.  

---

## ✅ Results
- **Best local accuracy:** ~85% (cross-validation)  
- **Kaggle Public Leaderboard Score:** `0.76794` 

---

## 📂 Project Structure
├── data/
│ ├── train.csv
│ ├── test.csv
├── notebook/
│ └── titanic.ipynb 
├── submission/
│ └── submission.csv 
├── Visualizations/
│ └── images.png    #all charts and insight 
├── README.md
