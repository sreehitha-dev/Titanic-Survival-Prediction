# Titanic_ds_project
Applied DS concepts on Titanic dataset and extracted insights and predicted survival rate based on the dataset.

# 📌 Project Overview
This project performs end-to-end data analysis and machine learning on the Titanic dataset to predict passenger survival.

It covers:

- Data loading
Data cleaning
Exploratory Data Analysis (EDA)
Feature engineering
Data visualization
Machine learning model building
# 📂 Dataset
Dataset: Titanic dataset (loaded using Seaborn)
Total records: 891 rows × 15 columns
Features include:
Passenger details: age, sex, pclass
Family info: sibsp, parch
Ticket info: fare, embarked
Target variable: survived
# 🧹 Data Cleaning
Filled missing values in age using mean

Dropped remaining missing values (deck, embarked, etc.)

Converted categorical data into numeric:

sex: male → 0, female → 1
embarked: S → 0, C → 1, Q → 2
alone: True → 1, False → 0
# ⚙️ Feature Engineering
Created a new feature:

fam_size = sibsp + parch
This helps understand the impact of family size on survival.

# 📊 Exploratory Data Analysis (EDA)
Key Insights:
✅ Females had significantly higher survival rate than males
✅ Higher class passengers (1st class) survived more
✅ Higher fare is associated with higher survival
✅ Smaller families had better survival chances
Visualizations Used:
Bar plots (survival rate, gender)
Histograms (age distribution)
Box plots (fare vs class)
Pie chart (survival percentage)
Scatter plot (age vs fare)
# 🤖 Machine Learning Model
Model Used:
Logistic Regression
Steps:
Train-test split (80% training, 20% testing)
Model training using sklearn
Predictions on test data
# 📈 Results
Model accuracy:0.8048780487804879
Confusion matrix visualized using heatmap
# 🛠️ Tech Stack
Python
Pandas, NumPy
Seaborn, Matplotlib
Scikit-learn
# 📁 Project Files
Titanic_DS_project.ipynb → Main notebook
titanic.csv → Exported dataset
🚀 How to Run
Open the notebook in Google Colab / Jupyter Notebook
Run all cells step by step
View analysis, visualizations, and model results
