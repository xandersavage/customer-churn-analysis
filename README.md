# 📊 Customer Churn Analysis

This project analyzes customer churn data from a retail bank using comprehensive Exploratory Data Analysis (EDA). The goal is to uncover key patterns and drivers of churn, providing actionable insights to improve customer retention strategies.

---

## 📁 Project Structure

```
customer-churn-analysis/
│
├── data/            # Raw dataset(s)
├── notebooks/       # Jupyter notebooks for analysis
│   └── 01-eda-churn.ipynb
├── images/          # Saved plots and visualizations
├── reports/         # Generated EDA reports
├── requirements.txt # Project dependencies
└── README.md        # Project documentation
```

---

## 📊 Dataset

- **Rows:** ~10,000 customers
- **Columns:** 14 features (Age, Gender, Geography, Balance, Products, Tenure, Credit Score, Estimated Salary, etc.)
- **Target Variable:** `Exited` (1 = churned, 0 = stayed)

> Source: [Kaggle — Bank Customer Churn Dataset](https://www.kaggle.com/datasets/barelydedicated/bank-customer-churn-modeling)

---

## 🔎 Analysis Workflow

1. **Data Cleaning & Preprocessing**

   - Imputed missing values and standardized data types
   - Encoded categorical features (e.g., Gender, Geography)

2. **Univariate Analysis**

   - Explored distributions of numerical features (Age, Balance, Salary)
   - Assessed churn rates across categorical variables (Gender, Geography, Products)

3. **Bivariate & Multivariate Analysis**

   - Investigated relationships between churn and individual features (e.g., Age vs. Churn)
   - Explored interaction effects (e.g., Geography + Products + Churn)
   - Generated correlation heatmaps for numerical features

4. **Visualization**
   - Created bar plots, histograms, boxplots, and heatmaps
   - Visualized churn breakdown by categories

---

## 💡 Key Insights

- **Overall churn rate:** ~20%
- **Mid-aged customers (39–51)** have the highest churn rate
- Customers with **only 1 product** are significantly more likely to churn
- **Geography matters:** German and French customers show the highest churn
- **Product usage** is more predictive of retention than credit score alone
- Female customers have a slightly higher churn rate than males

---

## 📈 Visualizations

### Churn Rate

<img width="955" height="525" alt="churn rate" src="https://github.com/user-attachments/assets/33ead69a-29bd-415f-b1d9-df8f9c6667b4" />

### Age by Exited (Box Plot)

<img width="955" height="525" alt="age by exited box plot" src="https://github.com/user-attachments/assets/502b43df-c9a6-482e-8149-328e67e99d35" />

### Geography vs Product Churn

<img width="955" height="525" alt="geography vs product churn" src="https://github.com/user-attachments/assets/f80eeab7-7777-4511-be8b-9346d12076af" />

_See the `images/` folder for more plots and visualizations._

---

## 🚀 Next Steps

This project is EDA-focused, but future extensions could include:

- Building machine learning models (e.g., Logistic Regression, Random Forest, XGBoost) to predict churn
- Advanced feature engineering (e.g., customer activity scores, segmentation)
- Designing and testing retention strategies for high-risk groups

---

## ⚙️ Tech Stack

- **Python:** pandas, numpy, matplotlib, seaborn, plotly
- **Jupyter Notebook** for analysis
- **GitHub** for version control and sharing

---

## 📌 How to Run

Clone the repository and install dependencies:

```bash
git clone https://github.com/xandersavage/customer-churn-analysis.git
cd customer-churn-analysis
pip install -r requirements.txt

jupyter notebook notebooks/01-eda-churn.ipynb
```

Open the notebook and follow the analysis steps. All required data and images are included in the respective folders.

---

## 📬 Contact

For questions or collaboration, feel free to reach out via GitHub Issues or connect on LinkedIn.
