# 🚢 Titanic Dataset – Exploratory Data Analysis (EDA)

This repository contains a complete **Exploratory Data Analysis (EDA)** of the famous **Titanic dataset**, one of the most iconic datasets in data science and machine learning.
The goal of this project is to uncover meaningful patterns, visualize relationships, and better understand the factors that influenced passenger survival during the tragic sinking of the RMS Titanic in 1912.

---

## 📌 Project Overview

The Titanic dataset provides demographic and travel information of passengers aboard the ship. Through detailed EDA, this project uncovers how variables such as **sex**, **age**, **family size**, **class**, **fare**, and **boarding location** impacted survival rates.

This project includes:

* Data loading & cleaning
* Univariate, bivariate & multivariate analysis
* Feature engineering
* Statistical summaries
* Visualizations using Matplotlib and Seaborn
* Survival insights supported by data

---

## 📁 Dataset

The project uses the **train.csv** file from the Kaggle Titanic dataset.
If you want to download the full dataset, grab it from:
👉 [https://www.kaggle.com/competitions/titanic/data](https://www.kaggle.com/competitions/titanic/data)

---

## 🧰 Technologies Used

| Purpose             | Tools/Libraries                 |
| ------------------- | ------------------------------- |
| Data manipulation   | **Pandas**, **NumPy**           |
| Visualization       | **Matplotlib**, **Seaborn**     |
| Environment         | Jupyter Notebook                |
| Feature engineering | Custom logic (Python functions) |

---

## 📊 Key Insights From the Analysis

### **1. Gender Had a Massive Impact on Survival**

The principle of *"Women and children first"* is clearly visible in the data:

* **≈74.2% of females survived**
* **≈18.9% of males survived**
* Passengers with the title **"Mrs"** showed the highest survival rate (**≈79.2%**)

### **2. Boarding Location & Class Influenced Fate**

* Passengers boarding at **Cherbourg (C)** had the **highest survival rate (≈55.4%)**
* Cherbourg also had **≈50.6% 1st-class passengers**
* Higher fare & 1st class were strongly correlated with survival

### **3. Family Size Played a Crucial Role**

A new feature, **Family Type**, was engineered:

* **Small families** had the best survival rate (**≈57.9%**)
* **Alone travelers**: **≈30.4% survival**
* **Large families**: **≈16.1% survival**

### **4. Age & Fare Distributions**

* Age is *almost normally distributed*, but ~20% values were missing
* Fare distribution is *highly positively skewed*
* Outliers indicate socioeconomic diversity
* Missing fare values were corrected with an **individual fare feature**

---

## 🧪 Feature Engineering

### ✔️ **Family Size**

Created by combining *SibSp* and *Parch*:

```
FamilySize = SibSp + Parch + 1
```

### ✔️ **Family Type**

```
Alone      → FamilySize = 1  
Small      → FamilySize 2–4  
Large      → FamilySize ≥ 5
```

### ✔️ **Individual Fare**

Divides fare by total family size to get more meaningful comparison.

---

## 📈 Visualizations Included

This project includes a series of detailed plots:

* Histograms for Age, Fare
* KDE plots
* Boxplots for outlier analysis
* Survival count plots
* Heatmaps for feature correlations
* Crosstab-based survival visualizations
* Distribution analysis by class, sex, age, and family size

These visualizations reveal patterns that are not obvious from raw data alone.

---

## 🗂 Repository Structure

```
Titanic-EDA/
│── EDA_On_Titanic_data.ipynb   # Main analysis notebook
│── train.csv                   # Dataset (if included)
│── README.md                   # Documentation
└── assets/                     # Optional: images & visualizations
```

---

## 🚀 How to Run the Notebook

1. **Clone the repository**

```
git clone https://github.com/your-username/Titanic-EDA.git
```

2. **Navigate into the project folder**

```
cd Titanic-EDA
```

3. **Install dependencies**

```
pip install -r requirements.txt
```

4. **Open the Jupyter Notebook**

```
jupyter notebook
```

---

## 📚 What You Will Learn

By exploring this notebook, you will understand:

* How to conduct structured EDA
* How to find hidden patterns in real-world datasets
* How to clean, preprocess, and visualize data
* How human decisions and social structures shape data outcomes
* The importance of feature engineering for ML readiness

---

## 🤝 Contributing

Contributions are always welcome!
If you'd like to improve visualizations, add ML models, or extend the analysis, feel free to open a pull request.

---

## ⭐ Support

If you found this project useful:

* ⭐ Star the repository
* 🔄 Share it with others
* 🧩 Fork the repo and build your own ML model on top of it

---

## 📬 Contact

If you want to collaborate or discuss data science ideas, feel free to connect:

📨 Email: *mdfirdaushusasain841@gmail.com*
🔗 LinkedIn: *www.linkedin.com/in/md-firdaus-hussain-a60b37282*


