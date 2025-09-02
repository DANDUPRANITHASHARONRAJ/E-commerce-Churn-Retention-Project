# E-commerce-Churn-Retention-Project

Project Overview:
This project aims to analyze customer behavior, identify churn drivers, and build predictive models to forecast churn in e-commerce platforms. Using real-world datasets from platforms like Flipkart, Amazon, and Nykaa, this project covers the full data analytics lifecycle: data collection, preprocessing, exploratory analysis, modeling, and deployment.


🔹 Week-wise Deliverables
Week 1 – Data Collection

Collected product, pricing, review, and transaction data using:

requests + BeautifulSoup → static pages

Selenium → dynamic pages & reviews

Saved datasets in CSV:

customers.csv, transactions.csv, products.csv
Columns: customer_id, product_id, order_date, price, rating, discount, delivery_time

Week 2 – Data Cleaning & Preprocessing

Handled missing values (fillna, dropna) and duplicates.

Converted dates into datetime format.

Normalized categorical columns (product categories, city, etc.).

Optional: Stored cleaned data in SQLite/MySQL database.

Week 3 – Exploratory Data Analysis (EDA)

Defined churn: Customers inactive for 60–90 days.

Key Metrics Calculated:

Total orders, Average basket value, Repeat rate

Visualizations using Seaborn & Matplotlib:

Histograms: Purchase frequency

Boxplots: Discounts vs churn

Cohort analysis: Retention trends by first purchase month

Week 4 – Root Cause Analysis (RCA)

Correlation analysis to detect churn drivers:

Delivery time, discount %, reviews

Hypothesis testing using scipy.stats.ttest_ind:

Churned vs retained: Delivery times

Churn vs review ratings

Documented top 3 churn drivers.

Week 5 – Baseline Modeling

Features engineered:

Recency, Frequency, Monetary (RFM)

Avg. delivery delay

Discount % usage

Logistic Regression (sklearn):

Train/test split: 80/20

Metrics: Accuracy, Precision, Recall, ROC-AUC

Week 6 – Advanced Modeling

XGBoost Classifier:

Compared performance vs Logistic Regression

Feature importance visualized using XGBoost & SHAP

Saved model: xgboost_model.pkl

Week 7 – Dashboarding (Power BI)

Created interactive dashboard:

KPI Cards: Retention %, Churn %, CLV

Line Chart: Retention over time

Funnel Chart: Visits → Cart → Purchase → Repeat

Heatmap: Churn % by city/category

Week 8 – Deployment & Packaging

Streamlit app:

Upload CSV

Run churn model

Show churn risk (High/Medium/Low)

GitHub repo includes:

Cleaned data, notebooks, models, Streamlit app, Power BI dashboards

Visuals exported to PPT/Figma for presentation.

🛠 Tools & Technologies

Languages & Libraries: Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Selenium, BeautifulSoup, SciPy

Databases: SQLite / MySQL (optional)

Visualization & Dashboarding: Power BI, Matplotlib, Seaborn

Deployment: Streamlit, GitHub

📈 Key Insights

Customers with delayed deliveries are more likely to churn.

Heavy discount usage correlates with higher churn.

Poor product reviews increase churn probability.

Cohort analysis shows retention drops sharply after 2 months of inactivity.
