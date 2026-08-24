# Customer Segmentation using K-Means Clustering

A machine learning project that segments retail customers into meaningful groups using **K-Means Clustering**, enabling data-driven, personalized marketing strategies.

## 📌 Overview

Businesses often apply the same marketing strategy to every customer, regardless of income, spending habits, or loyalty — leading to poor engagement and wasted marketing spend. This project uses **unsupervised machine learning** to solve that problem by grouping customers based on shared characteristics, so businesses can target each segment with tailored strategies.

## 🎯 Objectives

- Understand customer demographics and spending behavior through EDA
- Preprocess and scale customer data for clustering
- Determine the optimal number of clusters using the **Elbow Method**
- Build a **K-Means Clustering** model to segment customers
- Translate clusters into actionable business recommendations

## 🗂️ Dataset Features

The dataset includes the following customer attributes:
- Age
- Gender
- Annual Income
- Spending Score
- Membership Years

## 🔧 Methodology

1. **Data Cleaning** – handled missing values, removed duplicates, corrected data types, encoded categorical variables (Label Encoding for Gender)
2. **Exploratory Data Analysis (EDA)** – distribution plots, pair plots, and correlation heatmap to understand relationships between features
3. **Feature Scaling** – applied `StandardScaler` to normalize numerical features for accurate distance-based clustering
4. **Optimal Cluster Selection** – used the **Elbow Method** (WCSS vs K) to identify the ideal number of clusters
5. **Model Building** – trained a `KMeans` model to assign each customer to a cluster
6. **Cluster Analysis** – profiled each segment by average age, income, spending score, and membership duration

## 📊 Results: Customer Segments

The model identified **4 distinct customer segments**:

| Segment | Characteristics | Recommended Strategy |
|---|---|---|
| **Premium Customers** | High income, high spending, long membership | VIP memberships, exclusive discounts, early product access |
| **Budget Customers** | Low income, low spending | Coupons, cashback offers, affordable product bundles |
| **High Spenders** | High spending relative to income | Personalized recommendations, cross-selling, upselling |
| **New Customers** | Shorter membership duration | Welcome discounts, referral bonuses, onboarding offers |

## 🛠️ Tech Stack

- **Python**
- **Pandas** & **NumPy** – data manipulation
- **Matplotlib** & **Seaborn** – visualization
- **Scikit-learn** – `KMeans`, `StandardScaler`, `LabelEncoder`

## 📁 Repository Structure

```
├── Customer_Segmentation.ipynb      # Main analysis & clustering notebook
├── Project_report_final.docx        # Detailed project report
├── Project_Presentation.pptx        # Presentation summarizing the project
└── README.md                        # Project documentation
```

## ▶️ How to Run

1. Clone this repository
   ```
   git clone <repo-url>
   ```
2. Install dependencies
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Open `Customer_Segmentation.ipynb` in Jupyter Notebook and run all cells

## 📄 Project Report & Presentation

- Full write-up: `Project_report_final.docx`
- Summary slides: `Project_Presentation.pptx`

---
*This project was completed as part of an internship/academic machine learning module, applying unsupervised learning techniques to a real-world business use case.*
