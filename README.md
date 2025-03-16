# Cost-Profit-Analysis-And-Profit-Prediction-For-Food-Orders

This project analyzes food orders in New Delhi to assess profitability and predict profit using Linear Regression. It evaluates costs like order value, delivery fees, and discounts, providing insights to optimize pricing and maximize revenue.

The dataset contains 1,000 food order records with 12 columns, including order details, financial transactions, and payment processing information. Key columns for analysis include:
•	Order Value: Revenue from each order.
•	Delivery Fee: Cost of delivery.
•	Commission Fee: Platform's commission on the order.
•	Payment Processing Fee: Transaction fee.
•	Refunds/Chargebacks: Losses due to refunds.

The notebook includes standard data analysis libraries (numpy, pandas, matplotlib, seaborn). The first few code cells indicate:
1.	Data Loading: The dataset is loaded from a local path (food_orders_new_delhi.csv).
2.	Data Inspection: Basic dataset information (info()) and missing value checks (isnull().sum()) are performed.
3.	Customer Analysis: The notebook counts orders per customer (value_counts() on Customer ID).

The notebook focuses on customer behavior and restaurant order frequency using bar plots and pie charts. However, I haven't yet found direct cost-profit calculations or a machine learning model.

The notebook includes cost-related analysis (e.g., Order Value, Delivery Fee, Commission Fee, Payment Processing Fee, and Refunds/Chargebacks). 
Findings from the Analysis
1.	Cost-Profit Calculation: 
- The notebook correctly calculates profit using: 
-	Profit = Order Value - (Delivery Fee + Commission Fee + Payment Processing Fee) 
-	Discounts are considered, with a function handling percentage-based and fixed discounts.
2.	Customer & Market Insights: 
-	The notebook extracts valuable insights such as repeat customers, order frequency per restaurant, and peak order days.
-	Delivery fee impact, payment method preferences, and discount usage are well-analyzed.
3.	Machine Learning Model Implementation: 
-	Model Used: Linear Regression
-	Feature Engineering: 
  - Numerical features are standardized.
  - Categorical features (Payment Method, Meal, Delivery Day) are encoded.
- Train-Test Split: 80-20% split
- Performance Metrics: 
  - R-squared Score (r2_score)
  - Mean Squared Error (mse)
- Prediction Example: The model predicts profit for given input values.

Evaluation 
•	Data preprocessing, transformation, and training workflow are well-structured.
•	The cost-profit formula logically includes relevant cost components.
