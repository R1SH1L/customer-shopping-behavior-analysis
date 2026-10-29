**Customer Shopping Behavior Analysis**

An end-to-end Data Analytics and Business Intelligence project designed to analyze customer purchasing patterns, demographics, shipping preferences, and product ratings. This project transforms raw retail transaction data into actionable business insights using Python (Pandas & NumPy), SQL, and Power BI.

**Project Overview**

Retail businesses collect vast amounts of transactional data, but transforming this data into clear, strategic business strategy is often challenging. This project addresses core retail challenges:

* Demographic Targeting: Identifying high-value customer segments (age, gender, location).

* Behavioral Analysis: Examining the impact of subscriptions, promo code usage, and shipping methods on average purchase values.

* Product Strategy: Determining top-performing product categories and highly-rated items.

**Tech Stack & Tools**

* Programming / Data Analysis: Python 3.x, Pandas, NumPy, Jupyter Notebook

* Database Analysis: SQL (PostgreSQL / MySQL / SQLite)

* Data Visualization & BI: Microsoft Power BI, Power Query, DAX

* Version Control: Git, GitHub

**Dataset Information**

The analysis is conducted on a customer shopping dataset containing 3,900 purchase records with 18 attributes:

| Attribute | Description | 
| ----- | ----- | 
| Customer ID | Unique identifier for each customer | 
| Age / Gender / Location | Customer demographic details | 
| Item Purchased / Category | Purchased product and its high-level category | 
| Purchase Amount (USD) | Total transaction value | 
| Size / Color / Season | Product specification details | 
| Review Rating | Product rating given by customer (1 to 5) | 
| Subscription Status | Indicates whether the customer has an active subscription | 
| Payment Method / Shipping Type | Mode of payment and preferred shipping option | 
| Discount Applied / Promo Code Used | Details on discount or promotional offer usage | 
| Previous Purchases | Total number of past orders made by the customer | 

**Analytics Workflow**

1. Data Cleaning & Feature Engineering (Python):

   * Handled missing data and standardized schema headers.

   * Performed data type conversion and value consistency checks.

   * Created derived feature attributes like Age Group and Purchase Frequency Category.

2. Exploratory Data Analysis & Business Queries (SQL):

   * Extracted insights using Aggregations, GROUP BY, Window Functions, and CASE statements.

   * Evaluated total revenue distribution by gender, age bracket, and subscription status.

   * Measured discount dependency versus average order value (AOV).

3. Interactive Visualization (Power BI):

   * Built dynamic dashboards featuring multi-page reporting, custom DAX measures, tooltips, and slicers.

   * Modeled key metrics (Total Revenue, Average Purchase Amount, Subscription Conversion, Average Review Rating).

**Key Business Insights**

* Revenue Distribution: Young adults and mid-age groups represent the highest revenue-generating demographics.

* Shipping Impact: Customers selecting Express Shipping demonstrate a slightly higher average spend per transaction.

* Subscription Potential: A significant portion of repeat buyers do not currently hold an active subscription, representing an immediate opportunity for loyalty onboarding.

* Discount Drivers: Promotional codes drive high transaction volumes in specific categories (e.g., Clothing and Accessories) without drastically reducing unit value.

**Repository Structure**

```
customer-shopping-behavior-analysis/
├── customer_shopping_data.csv
├── customer_shopping_behavior.ipynb
├── sql_queries.sql
└── README.md
```

**How to Run & Reproduce**

**1. Clone the Repository**

```
git clone https://github.com/R1SH1L/customer-shopping-behavior-analysis.git
cd customer-shopping-behavior-analysis
```

**2. Python Environment Setup**

```
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

pip install pandas numpy matplotlib seaborn jupyter
```

Run the Jupyter notebook to view the data cleaning process and initial exploratory analysis.

**3. Database Query Execution**

1. Load `customer_shopping_data.csv` into your preferred SQL database engine (MySQL, PostgreSQL, or SQLite).

2. Run the queries provided in `sql_queries.sql` to execute the business logic.

**Contributing**

Contributions, feedback, and pull requests are welcome. Feel free to open an issue or submit a PR.

**License**

This project is licensed under the MIT License.
