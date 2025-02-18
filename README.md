# Project_1-E-commerce-Customer-Behavior-Analysis
Project Overview
This project focuses on analyzing customer behavior within an e-commerce platform using a dataset that captures various customer attributes and their purchasing patterns. The goal is to uncover insights that can help the business make data-driven decisions to enhance customer experience, optimize marketing strategies, and improve customer retention.

Dataset Description
The dataset, E-commerce Customer Behavior, contains 350 observations (customers) and 11 variables. Each row represents a unique customer, and the columns provide detailed information about their demographics, purchasing behavior, and satisfaction levels.
Variables:
    1. Customer ID: Unique identifier for each customer.
    2. Gender: Categorical variable (Male, Female).
    3. Age: Numeric variable representing the customer's age.
    4. City: Categorical variable indicating the customer's city of residence (Chicago, Houston, Los Angeles, Miami, New York, San Francisco).
    5. Membership Type: Categorical variable (Gold, Silver, Bronze) indicating the customer's membership level.
    6. Total Spend: Numeric variable representing the total monetary expenditure by the customer.
    7. Items Purchased: Numeric variable indicating the total number of items purchased.
    8. Average Rating: Numeric variable (0 to 5) representing the average rating given by the customer.
    9. Discount Applied: Boolean variable (True, False) indicating whether a discount was applied.
    10. Days Since Last Purchase: Numeric variable indicating the number of days since the customer's last purchase.
    11. Satisfaction Level: Categorical variable (Satisfied, Neutral, Unsatisfied) capturing the customer's overall satisfaction.

Project Structure
The project is divided into the following sections:
1. Data Loading and Preprocessing
    • The dataset is loaded and categorical variables (Gender, City, Membership Type, Satisfaction Level) are converted into factors for analysis.
    • Basic exploratory data analysis (EDA) is performed to understand the structure and distribution of the data.
2. Univariate Analysis
    • Gender: The dataset is balanced, with an equal number of male and female customers.
    • City: Customers are distributed across six cities, with New York and Los Angeles having the highest representation (16.9% each).
    • Membership Type: The distribution of membership types is almost equal (33.1% Bronze, 33.4% Gold, 33.4% Silver).
    • Satisfaction Level: Most customers are satisfied (35.7%), followed by neutral (30.6%) and unsatisfied (33.1%). A small percentage (0.6%) did not provide their satisfaction level.
    • Age: Customers are predominantly young to middle-aged adults, with ages ranging from 26 to 43 years.
    • Total Spend: There is a wide range of spending, with some customers spending significantly more than others.
    • Items Purchased: The number of items purchased varies, with satisfied customers purchasing more items on average.
3. Bivariate Analysis
- A correlation matrix is used to explore relationships between numerical variables:
        ◦ Total Spend and Average Rating have a strong positive correlation (0.94).
        ◦ Age is negatively correlated with Average Rating (-0.72) and Total Spend (-0.68).
        ◦ Days Since Last Purchase is negatively correlated with Total Spend (-0.54).
  - In average Gold (more than $1250 ) menbership spend more than silver (almost $750) and Bronze (less than $500). The Gold is our potential clients that spend a lot in our shop.
 - Men tend to spend more than women.
 - San Francisco ($1459,772) is the biggest spender, followed by New York (average $1165,036) and Houston (less than $500).
 - The average spending of those aged between 26 and 30 is very different from that of those aged between 31 and 43.
4. Expenditure Analysis
    • Membership Type: Gold members spend significantly more (1250onaverage)comparedtoSilver(750) and Bronze ($500) members.
    • City: Customers from San Francisco spend the most (1459.77onaverage),followedbyNewYork(1165.04). Houston has the lowest average spending.
    • Gender: Men tend to spend slightly more than women.
    • Age: Customers aged 26-30 spend more on average than those aged 31-43.
5. Forecasting with Linear Regression
    • A linear regression model is built to predict Total Spend based on customer attributes.
    • Key findings:
        ◦ Age: Each additional year of age increases total spending by 1.74 units.
        ◦ City: Customers in San Francisco and New York spend significantly more.
        ◦ Items Purchased: Each additional item purchased increases total spending by 25.33 units.
        ◦ Days Since Last Purchase: Each additional day since the last purchase decreases total spending by 1.28 units.

Key Insights
    1. Priority Targets:
        ◦ Customers in San Francisco and New York are high spenders and should be targeted for premium offers.
        ◦ Gold members and customers who purchase more items are also high-priority targets.
    2. Loyalty Programs:
        ◦ Customers who return frequently (fewer days since last purchase) spend more. Loyalty programs can encourage repeat purchases.
    3. Gender-Neutral Strategies:
        ◦ Gender does not significantly impact spending, so marketing strategies should not be differentiated by gender.
    4. Satisfaction Drives Purchases:
        ◦ Satisfied customers tend to purchase more items. Improving customer satisfaction can directly boost sales.

Tools and Libraries Used
    • R Programming Language
    • Libraries:
        ◦ dplyr: For data manipulation.
        ◦ ggplot2: For data visualization.
        ◦ scales: For formatting percentages in visualizations.
        ◦ corrplot: For visualizing correlation matrices.
        ◦ lm: For building linear regression models.

How to Run the Code
    1. Clone the repository or download the R script and dataset.
    2. Open the R script in RStudio.
    3. Ensure the dataset (E-commerce_Customer_Behavior.csv) is in the working directory.
    4. Install the required libraries if not already installed:
       R
       Copy
       install.packages(c("dplyr", "ggplot2", "scales", "corrplot"))
    5. Run the script to generate the analysis and visualizations.

Conclusion
This project provides actionable insights into customer behavior, helping the e-commerce platform optimize its marketing strategies, improve customer satisfaction, and increase revenue. By focusing on high-spending segments and implementing targeted loyalty programs, the business can enhance its overall performance.
