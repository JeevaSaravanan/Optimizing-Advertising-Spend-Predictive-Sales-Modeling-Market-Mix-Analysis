# **Optimizing Advertising Spend: Predictive Sales Modeling & Market Mix Analysis**

## **Project Overview**
This project analyzes the impact of advertising spend across multiple channels on product sales. Using **Machine Learning models and statistical analysis**, we aim to **optimize budget allocation** and **predict future sales** effectively.

## **Project Goals**
- Identify **key advertising channels** that drive the most sales.
- Use **Market Mix Modeling (MMM)** to optimize advertising budget allocation.
- Develop **predictive models** using **XGBoost, LightGBM, and CatBoost**.
- Utilize **SHAP analysis** to interpret model decisions and advertising impact.
- Provide actionable insights to improve marketing efficiency.

---

## **Dataset Overview**
- **File Name:** `Advertising_Data.csv`
- **Rows:** 300
- **Columns:**
  - TV Advertising Cost
  - Billboard Advertising Cost
  - Google Ads Cost
  - Social Media Spend
  - Influencer Marketing Spend
  - Affiliate Marketing Spend
  - **Product_Sold (Target Variable)**
- **Purpose:** Understanding the impact of advertising spend on sales.

---

## **Key Analysis & Methods**
### **1. Exploratory Data Analysis (EDA)**
- Data cleaning, summary statistics, and correlation heatmaps.
- Feature distribution analysis and scatter plots to detect trends.

![alt text](image.png)

![alt text](image-1.png)

### **2. Feature Importance (SHAP Analysis)**
**Insights from Feature Importance & SHAP Analysis**

**Feature Importance (Random Forest)**
- **Affiliate Marketing** is the most influential factor, driving the highest impact on sales.
- **Billboards and Social Media** also have significant effects, meaning traditional and digital advertising both play key roles.
- **TV and Google Ads** contribute moderately to sales but are not the primary drivers.
- **Influencer Marketing** has the least impact, suggesting it may not be an effective use of the budget.

**SHAP Beeswarm Plot**
- **Higher values of Affiliate Marketing spending strongly increase sales**, confirming its importance.
- **Billboards and Social Media have mixed effects**, where spending more does not always guarantee higher sales.
- **TV Ads and Google Ads show diminishing returns**, indicating that past a certain point, increasing spend does not significantly boost sales.
- **Influencer Marketing has mostly negative or low impact**, meaning increasing its budget may not lead to better results.

![alt text](image-2.png)
![alt text](image-3.png)

### **3. Market Mix Modeling (MMM)**
- Built a **Multiple Linear Regression model** to analyze ROI on advertising spend.
- Found optimal budget allocations for different ad platforms.
    
- The Multiple Linear Regression Model estimates how each advertising channel contributes to Product Sold:

**Key Results:**  

- Affiliate Marketing (coef: ~3.99) → Highest impact on sales.
- Billboards (coef: ~2.99) → Significant effect on product sales.
- Social Media (coef: ~2.50) → Contributes well to sales.
- TV (coef: ~2.00) → Moderate impact on sales.
- Google Ads (coef: ~1.50) → Lower impact than expected.
- Influencer Marketing (coef: ~1.20) → Least effective channel.

### **4. Predictive Sales Modeling**
Trained multiple **Machine Learning models** with **hyperparameter tuning** to predict sales:
- **Best Performing Model:** **CatBoost (R² = 0.9447, RMSE = 397.9)**
- Other strong models: **LightGBM, Gradient Boosting, and XGBoost.**
- **Linear Regression showed overfitting, and Support Vector Regression performed poorly.**

---

## **Results & Key Insights**
- **Affiliate Marketing, Billboards, and Social Media drive the most sales.**  
- **Influencer Marketing has minimal impact and may not be an effective budget allocation.**  
- **CatBoost is the best predictive model for accurate sales forecasting.**  
- **Market Mix Modeling suggests redistributing budget towards high-impact channels.**

---

## **How to Use This Project**
1. **Data Preparation:** Load `Advertising_Data.csv` into a Pandas DataFrame.
2. **Run EDA & Feature Importance Analysis** using `seaborn` & `SHAP`.
3. **Train Machine Learning models** to predict `Product_Sold`.
4. **Interpret feature importance** and adjust marketing strategies accordingly.

---

## **Technologies Used**
- Python (pandas, numpy, matplotlib, seaborn, sklearn, statsmodels, shap)
- **Machine Learning Models:** XGBoost, LightGBM, CatBoost, Random Forest, Gradient Boosting
- **Statistical Modeling:** Multiple Linear Regression (MMM)

---

## **Contributors**
- **Project Owner:** Jeeva Saravana Bhavanandam

<div align="center">

<a href="https://jeevasaravanan.medium.com/" target="_blank">![Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)</a> <a href="https://www.linkedin.com/in/jeeva-saravanan/" target="_blank">![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)</a> <a href="https://jeeva-saravana-bhavanandam.web.app" target="_blank">![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=GoogleChrome&logoColor=white)</a>


</div>

