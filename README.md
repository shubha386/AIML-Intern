# 🧼 Titanic Dataset - Data Cleaning & Preprocessing Task

This project is part of an ML internship task focused on data cleaning and preprocessing.  
The dataset used is the **Titanic Dataset**, and the goal is to prepare it for machine learning models by performing the following key steps:

---

## ✅ Task Objectives (as per guide)
1. **Import the dataset and explore basic info**
2. **Handle missing values using mean/median/imputation**
3. **Convert categorical variables using encoding**
4. **Normalize/standardize numerical features**
5. **Visualize outliers using boxplots and remove them**

---

## 🧪 Steps Performed

### 1. Data Loading & Exploration
- Loaded dataset using `pandas`.
- Used `df.info()`, `df.describe()`, and `df.isnull().sum()` to explore structure and missing values.

### 2. Missing Value Handling
- Filled missing `Age` values using **median**.
- Filled missing `Embarked` values using **mode**.
- Dropped `Cabin` column due to high percentage of missing data.

### 3. Feature Selection
- Dropped irrelevant columns: `Name`, `Ticket`.

### 4. Encoding Categorical Variables
- Encoded `Sex` using **label encoding**: `male` → 0, `female` → 1.
- Used **one-hot encoding** on `Embarked` with `drop_first=True`.

### 5. Standardization
- Scaled numerical features `Age` and `Fare` using `StandardScaler`.

### 6. Outlier Detection & Removal
- Used **boxplot** to visualize `Fare` outliers.
- Removed outliers using the **Interquartile Range (IQR)** method.

---

## 📁 Files Included
- `preprocessing.py`: Full preprocessing script.
- `Titanic-Dataset.csv`: Raw dataset (if allowed).
- `cleaned_titanic.csv`: Cleaned dataset (optional, if saved).
- `README.md`: Project summary (this file).
- `screenshots/`: Plots and visualizations (optional).

---

## 🚀 Tools Used
- Python
- Pandas
- Seaborn & Matplotlib (for visualization)
- scikit-learn (for scaling)

---

## 📌 Author
- **Subathra Mahalakshmi**  
- Internship Task Submission | AIML
