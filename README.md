Titanic Exploratory Data Analysis (EDA)

📊 Project Goal
The objective of this project is to perform a comprehensive Exploratory Data Analysis (EDA) on the Titanic dataset to uncover hidden patterns, detect missing values, study feature distributions, and identify key factors influencing survival.

📂 Dataset

The dataset is the classic Titanic: Machine Learning from Disaster
 dataset from Kaggle.

train.csv – training data with passenger details and survival labels

test.csv – test data (without survival labels)

gender_submission.csv – sample submission file

Key Features:

Survived: Survival (0 = No, 1 = Yes)

Pclass: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)

Sex: Gender of passenger

Age: Age in years

SibSp: Number of siblings/spouses aboard

Parch: Number of parents/children aboard

Fare: Ticket fare

Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

Cabin: Cabin number (mostly missing)

Name and Ticket: Identifier information

🔎 Analysis Workflow

Data Understanding

Checked shape, column types, summary statistics

Identified missing values (Cabin, Age, Embarked)

Univariate Analysis

Histograms for numerical features (Age, Fare, SibSp, Parch)

Value counts for categorical variables (Sex, Pclass, Embarked, Survived)

Bivariate Analysis

Boxplots: Fare vs Pclass, Age vs Survived

Crosstabs: Survival by Sex and Pclass

Correlation Analysis

Heatmap of numeric features

Scatter plots (e.g., Age vs Fare colored by survival)

Pairwise scatter matrix

Insights & Observations

Cabin is almost entirely missing → needs dropping or advanced feature engineering.

Age has ~177 missing values → imputation required (median or model-based).

Gender: Survival rate → Females: 74%, Males: 19%.

Class: Survival rate → 1st: 63%, 2nd: 47%, 3rd: 24%.

Fare positively correlated with survival; Pclass negatively correlated.

SibSp and Parch moderately correlated (Family-size signal).

📑 Deliverables

Notebook: Titanic_EDA.ipynb – full analysis with code & plots

Final PDF Report: Titanic_Final_Report.pdf – insights + all charts in order

Script: titanic_eda_script.py – lightweight reproducible script

Visuals: Histograms, bar charts, boxplots, scatter plots, correlation matrix

🚀 Next Steps

Handle missing values (Age, Embarked)

Feature engineering: extract Title from Name, compute FamilySize (SibSp + Parch + 1), encode Embarked, one-hot encode categorical features

Model building: Logistic Regression, Random Forest, Gradient Boosting

Evaluate with accuracy, ROC-AUC, and explainability tools (e.g., SHAP)

👨‍💻 Author

Manish Kumar Gangala

Gmail : gangamanishkumar@gmail.com

LinkedIn : www.linkedin.com/in/manish-kumar-gangala-095a2224a
