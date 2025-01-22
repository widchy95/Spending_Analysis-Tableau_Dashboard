# Payment Method Preference Analysis

This project explores customer payment method preferences and their relationship with transaction types using a synthetic Spending Patterns Dataset. The dataset consists of 10,000 transactions for 200 unique customers, providing insights into consumer behavior across various spending categories.

## Dataset Overview

The dataset includes the following key features:
- **Customer ID**: Unique identifier for each customer (e.g., CUST_0001).
- **Category**: Spending category (e.g., Groceries, Travel, Shopping).
- **Item**: Specific item purchased within a category (e.g., Milk, Plane Ticket).
- **Quantity**: Number of units purchased.
- **Price Per Unit**: Price of one unit of the item (in USD).
- **Total Spent**: Total expenditure for the transaction (Quantity × Price Per Unit).
- **Payment Method**: Payment method used (e.g., Credit Card, Cash).
- **Location**: Transaction location (e.g., Online, In-store, Mobile App).
- **Transaction Date**: Date of the transaction (YYYY-MM-DD format).

## Objectives

The primary goal of this analysis is to:
1. Calculate the proportion of each payment method used across transactions.
2. Explore payment preferences by spending category, transaction location, and spending amount.
3. Perform statistical tests to identify significant relationships between payment methods and other features (e.g., categories, locations).
4. Exclude the "Shopping" category from the analysis for a focused study on other spending behaviors.

## Analysis Steps

### 1. Proportion of Payment Methods
- Calculated the proportion of transactions using each payment method.
- Visualized the overall distribution with a **pie chart**.

### 2. Payment Method Preferences by Category and Location
- Aggregated total spending by payment method for each category and location.
- Filtered out the "Shopping" category to focus on other areas.
- Visualized preferences with **stacked bar charts**.

### 3. Spending Amount Distribution
- Used **boxplots** to analyze spending amount distributions by payment method.

### 4. Statistical Testing
- Conducted **Chi-square tests** to determine:
  - Whether payment method preferences vary significantly by category.
  - Whether payment method preferences vary significantly by location.

## Key Findings

1. **Payment Method Proportions**:
   - Identified the most and least preferred payment methods among customers.

2. **Category and Location Analysis**:
   - Highlighted trends in payment methods for specific categories and locations.
   - Found that preferences differ significantly between locations such as online, in-store, and mobile app transactions.

3. **Spending Amount Insights**:
   - Observed that spending amounts vary widely across payment methods.
   - Certain methods like credit cards were more associated with higher spending transactions.

4. **Statistical Significance**:
   - Detected a statistically significant relationship between payment method preferences and transaction categories.
   - Found no significant relationship between payment methods and transaction locations.

## Visualizations

- **Pie Chart**: Overall payment method distribution.
- **Stacked Bar Charts**:
  - Payment method preferences by category (excluding "Shopping").
  - Payment method preferences by location.
- **Boxplot**: Spending amount distribution by payment method.

## Tools and Libraries

- **Programming Language**: Python
- **Libraries**:
  - Pandas: Data manipulation and aggregation
  - Matplotlib and Seaborn: Data visualization
  - SciPy: Statistical testing (Chi-square test)

## How to Run the Analysis

1. Clone the repository:
   ```bash
   git clone https://github.com/widchy95/Spending_Analysis-Tableau_Dashboard.git
   cd payment-method-analysis
   ```
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn scipy
   ```
3. Run the analysis script:
   ```bash
   python payment_analysis.py
   ```
4. View the visualizations generated in the project directory.

## Future Improvements

- Incorporate demographic data for deeper insights into payment preferences.
- Apply machine learning models to predict payment method preferences.
- Explore seasonal effects on spending and payment behaviors.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

- Synthetic dataset provided for educational and analytical purposes.
- Inspired by real-world financial analysis scenarios.

