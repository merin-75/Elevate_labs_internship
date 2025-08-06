# 🧹 Task 1: Data Cleaning & Preprocessing

## 🎯 Objective
Learn how to clean and prepare raw data for machine learning tasks using Python and data science libraries.

---

## 📦 Dataset Used
**Titanic Dataset**  
Source: [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data)  
Alternate: Loaded directly from GitHub:  
`https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv`

---

## 🧰 Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📝 Steps Performed

### ✅ 1. Import and Explore Dataset
- Used `pandas` to load Titanic dataset from an online source.
- Explored structure, datatypes, and missing values using:
  - `df.head()`
  - `df.info()`
  - `df.describe()`
  - `df.isnull().sum()`

### ✅ 2. Handle Missing Values
- Filled missing `Age` with **median**.
- Filled missing `Embarked` with **mode**.
- Dropped `Cabin` column due to excessive nulls.

### ✅ 3. Encode Categorical Variables
- Label encoded `Sex` column (`male=0`, `female=1`).
- One-hot encoded `Embarked` column (dropped first to avoid dummy variable trap).

### ✅ 4. Normalize/Standardize Numerical Features
- Scaled `Age` and `Fare` using `StandardScaler` from `sklearn`.

### ✅ 5. Detect and Remove Outliers
- Visualized `Fare` outliers using `seaborn.boxplot()`.
- Applied **IQR method** to remove outliers.

