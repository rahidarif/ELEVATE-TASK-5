# Titanic Dataset Analysis  
A simple exploratory data analysis (EDA) project performed using **Python (Pandas, Matplotlib)** on the Titanic dataset.  
This analysis focuses on understanding passenger demographics, exploring variable distributions, identifying trends, and visualizing key relationships in the data.

---

## 📂 Project Overview
This project performs the following:
- Basic dataset inspection  
- Summary statistics  
- Exploratory data analysis using visualizations  
- Understanding relationships between age, fare, survival, and passenger class  

The project uses **only Matplotlib for visualizations**, following constrained environment rules.

---

## 📁 Dataset Description
The dataset contains information about **891 Titanic passengers** with the following key features:

| Column       | Description |
|--------------|-------------|
| Survived     | Survival (0 = No, 1 = Yes) |
| Pclass       | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| Name         | Passenger name |
| Sex          | Gender |
| Age          | Age in years |
| SibSp        | # of siblings/spouses aboard |
| Parch        | # of parents/children aboard |
| Ticket       | Ticket number |
| Fare         | Ticket fare |
| Cabin        | Cabin number |
| Embarked     | Port of Embarkation (C/Q/S) |

---

## 🧪 Steps Performed

### **1. Basic Data Exploration**
- `df.info()` – Shows column types and missing values  
- `df.describe()` – Generates summary statistics  
- `df['column'].value_counts()` – Used for `Sex`, `Pclass`, and `Embarked`

### **2. Visualizations (Matplotlib)**

#### **Histogram – Age Distribution**
- Shows the most common age range (20–40 years)
- Reveals missing age values

#### **Boxplot – Fare**
- Highlights right-skewed fare distribution  
- Shows many high-value outliers (mainly 1st class passengers)

#### **Scatter Plot – Age vs Fare**
- Used to explore relationship between passenger age and ticket fare  
- No strong correlation observed

#### **Correlation Heatmap (Matplotlib-based)**
- Shows correlations between numeric variables:  
  `Survived`, `Pclass`, `Age`, `SibSp`, `Parch`, `Fare`

#### **Scatter Matrix**
- Provides pairwise relationships similar to Seaborn’s pairplot

---

## 📊 Summary of Findings

- **Age Distribution:** Most passengers were between **20–40 years**, with fewer children and elderly individuals.
- **Fare Distribution:** Highly skewed with many outliers; 1st class passengers paid significantly more.
- **Age–Fare Relationship:** No strong pattern; both high and low fares occur across ages.
- **Passenger Classes:** Majority of travelers were from **3rd class**, affecting fare and survival patterns.
- **Missing Values:** Significant missing data in the **Cabin** column; moderate missing values in **Age**.

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- Matplotlib  
- Jupyter Notebook / Google Colab  

---

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/titanic-analysis.git
