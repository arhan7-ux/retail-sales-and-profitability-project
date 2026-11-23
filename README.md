PROJECT TITLE
retail-sales-and-profitability-project

BRIEF ONE LINE SUMMARY
An Exploratory Data Analysis project using Python to analyze retail sales transactions, identify top-performing product categories, understand customer purchasing behaviour, and uncover sales patterns through data visualization.

OVERVIEW
Retail Sales Data Analysis is a data analytics project developed to explore retail transaction data and extract meaningful business insights.

The project uses Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn to analyze sales performance, product categories, customer demographics, payment methods, discounts, and product ratings.

Through Exploratory Data Analysis (EDA), the project examines different aspects of retail business performance and presents findings through graphical visualizations.

The primary objective is to understand customer purchasing patterns, identify popular products, analyze sales distribution, and support data-driven business decisions.

PROBLEM STATEMENT
Retail businesses generate large amounts of transaction data, but extracting meaningful information from this data is essential for understanding business performance and customer behaviour.

The objective of this project is to analyze retail sales data to:

Identify product categories generating the highest sales revenue.

Analyze sales distribution across different payment methods.

Understand purchasing behaviour across customer demographics.

Identify the top-selling products based on total sales amount.

Explore the relationship between previous purchases and applied discounts.

Analyze average product ratings across different age groups.

Examine correlations between important numerical variables.

The project aims to transform raw retail transaction data into meaningful business insights through Python-based data analysis and visualization.

DATASET
Dataset Name: Retail Sales Dataset

File Name: store_sales.csv

Dataset Type: Structured Transactional Data

Dataset Attributes:

Column                  Description

CustomerID              Unique customer identification number

Age                     Age of the customer

Gender                  Gender of the customer

Category                Product category

ItemPurchased           Name of the purchased item

Amount                  Transaction amount

Season                  Season during which the purchase was made

PaymentMethod           Payment method used

ItemRating              Customer rating for the purchased item

DiscountApplied(%)      Discount percentage applied

PreviousPurchases       Number of previous purchases

Data Quality Assessment:

Examined dataset structure and column information.

Checked for duplicate records.

No duplicate records were identified.

Checked for missing values across all columns.

No missing values were identified.

Features Analyzed:

Sales Amount

Product Category

Customer Age

Gender

Payment Method

Product Ratings

Discount Percentage

Previous Purchases

Seasonal Purchasing Behaviour

TOOLS AND TECHNOLOGIES
Programming Language:

Python

Libraries and Frameworks:

Pandas – Data loading, manipulation, grouping, and aggregation.

NumPy – Numerical computations.

Matplotlib – Data visualization and graphical representation.

Seaborn – Statistical visualization and correlation analysis.

Development Environment:

Jupyter Notebook

Data Analytics Techniques:

Exploratory Data Analysis (EDA).

Data Cleaning and Validation.

Data Aggregation.

GroupBy Operations.

Statistical Analysis.

Correlation Analysis.

Data Visualization.

METHODS AND IMPLEMENTATION
The project follows these implementation steps:

Step 1: Data Collection and Loading

Imported the retail sales dataset from a CSV file using Pandas and loaded it into a DataFrame for analysis.

Step 2: Data Inspection

Examined the first five records using head().

Checked the dataset columns.

Reviewed the dataset structure.

Inspected the available customer and transaction attributes.

Step 3: Data Quality Assessment

Performed data quality checks to identify potential issues.

Checked duplicate records using duplicated().

Checked missing values using isnull().sum().

Verified the dataset columns.

The analysis identified zero duplicate records and zero missing values.

Step 4: Sales Analysis by Product Category

Used Pandas groupby() and sum() to calculate the total sales amount for each product category.

Created a bar chart to compare sales performance across categories.

Step 5: Discount and Previous Purchase Analysis

Created a scatter plot using Seaborn to explore the relationship between the number of previous purchases and the discount percentage applied.

Step 6: Payment Method Analysis

Grouped transaction amounts by payment method and generated a pie chart to visualize the contribution of different payment methods to total sales.

Step 7: Gender-Based Sales Analysis

Analyzed total sales amounts across gender categories using Pandas aggregation and pie chart visualization.

Step 8: Top 10 Product Analysis

Identified the top 10 purchased items based on their total transaction amount using groupby(), sum(), sort_values(), and head(10).

Visualized the results using a bar chart.

Step 9: Customer Age Group Analysis

Created a new feature called Age_Group using conditional logic.

The age groups were defined as:

Child: Age below 18.

Adult: Age from 18 to below 35.

Senior: Age 35 and above.

Step 10: Average Product Rating Analysis

Calculated the average item rating for each age group and visualized the results using a bar chart.

Step 11: Correlation Analysis

Generated a correlation matrix for the following numerical variables:

Amount

ItemRating

DiscountApplied(%)

PreviousPurchases

Created a Seaborn heatmap to visualize relationships between these variables.

KEY INSIGHTS
The project explores several important business dimensions:

1. Product Category Performance

Analyzed total sales amounts across different product categories to identify categories contributing the most revenue.

2. Customer Purchasing Behaviour

Examined previous purchase counts alongside applied discount percentages to understand their distribution and potential relationships.

3. Payment Method Preferences

Compared total transaction amounts across payment methods to understand their contribution to overall sales.

4. Gender-Based Sales Distribution

Analyzed sales amounts across gender categories to understand differences in purchasing contribution.

5. Top 10 Products

Identified the ten products generating the highest cumulative transaction amounts.

6. Age Group and Product Ratings

Compared average product ratings across the three age groups created during analysis.

7. Correlation Between Numerical Variables

Used a correlation heatmap to explore relationships among transaction amount, item ratings, discounts, and previous purchases.

These analyses provide a foundation for understanding retail performance, customer preferences, and purchasing patterns.

DASHBOARD / MODEL / OUTPUT
Project Type: Exploratory Data Analysis (EDA)

This project currently uses Python-based visualizations in Jupyter Notebook rather than a deployed dashboard or predictive Machine Learning model.

Visualizations Generated:
Visualization                                    Business Purpose

Bar Chart – Total Amount by Category             Compare category-wise sales

Scatter Plot – Previous Purchases vs Discount    Explore discount patterns

Pie Chart – Amount by Payment Method             Understand payment distribution

Pie Chart – Amount by Gender                     Compare gender-wise sales

Bar Chart – Top 10 Items by Amount               Identify high-revenue products

Bar Chart – Average Rating by Age Group          Compare customer ratings

Compare customer ratings                         Examine numerical relationships

Key Output:

The notebook generates seven visualizations that provide different perspectives on retail sales performance and customer purchasing behaviour.

The analysis helps identify important business patterns that can support sales optimization and customer-focused decision-making.

HOW TO RUN THIS PROJECT?
Follow these steps to execute the project locally.

Prerequisites:

Python 3.x

Jupyter Notebook

Basic knowledge of Python and Data Analytics

Step 1: Clone the Repository
git clone <your-repository-url>

Step 2: Navigate to the Project Directory
cd <your-project-folder>

Step 3: Install Required Libraries
pip install pandas numpy matplotlib seaborn jupyter

Step 4: Add the Dataset

Place the store_sales.csv file inside your project directory.

Update the dataset loading statement in the notebook:
import pandas as pd

df = pd.read_csv("store_sales.csv")

Step 5: Launch Jupyter Notebook
jupyter notebook

Step 6: Execute the Notebook

Open Retail Sales Project.ipynb and execute the cells sequentially.

The notebook will:

Load the retail sales dataset.

Perform data inspection and quality checks.

Analyze category-wise sales.

Explore discounts and previous purchases.

Examine payment method and gender-wise sales.

Identify the top 10 products.

Create customer age groups.

Analyze average product ratings.

Generate a correlation heatmap.

RESULTS AND DISCUSSION
The project successfully demonstrates how Python-based Exploratory Data Analysis can be used to investigate retail sales transactions and understand customer purchasing behaviour.

The analysis covers multiple business dimensions, including product category performance, payment methods, gender-based sales distribution, top-performing products, customer age groups, product ratings, and numerical correlations.

Seven different visualizations were developed using Matplotlib and Seaborn to communicate the results effectively.

The project demonstrates practical experience in:

Python programming.

Data cleaning and validation.

Exploratory Data Analysis.

Data aggregation and manipulation.

Customer behaviour analysis.

Statistical correlation analysis.

Data visualization.

Business insight generation.

Overall, the project demonstrates how raw retail transaction data can be transformed into structured information to support data-driven business decisions.

FUTURE WORK
The project can be enhanced through the following improvements:

Advanced Exploratory Data Analysis: Perform deeper analysis of seasonal trends, customer demographics, and product category performance.

Sales Trend Analysis: Analyze sales patterns across different seasons and time periods to identify revenue trends.

Customer Segmentation: Apply K-Means Clustering to group customers based on purchasing frequency, transaction amounts, and spending behaviour.

Interactive Dashboard: Develop an interactive Power BI or Tableau dashboard to present sales KPIs, category performance, and customer insights.

Advanced Statistical Analysis: Apply statistical techniques to investigate relationships between discounts, spending, and purchasing behaviour.

Sales Forecasting: Implement time-series forecasting techniques to estimate future sales trends, if suitable date-level data is available.

Business Recommendations: Develop actionable recommendations for product promotions, customer engagement, and sales optimization.

Automated Reporting: Create automated reports that summarize important sales metrics and business insights.

AUTHOR & CONTACT
Author: Arhan
Project: Retail Sales And Profitability Project
LinkedIn:www.linkedin.com/in/arhan-gogi-34aa992b9
Github:https://github.com/arhan7-ux
Email: arhangogi07@gmail.com

