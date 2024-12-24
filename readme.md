# Sales Data Analysis

This repository contains a comprehensive analysis of sales data using Jupyter Notebooks. The analysis includes data preprocessing, time series decomposition, and various visualizations to understand the sales trends, deviations, and forecast accuracy.

## Repository Structure

- [`analysis.ipynb`](analysis.ipynb): Jupyter Notebook for data preprocessing, time series decomposition, and initial analysis.
- [`Charts.ipynb`](Charts.ipynb): Jupyter Notebook for generating various visualizations and charts based on the processed data.
- [`priority_data_fixed.csv`](priority_data_fixed.csv): CSV file containing prioritized sales data with deviation categories and priorities.
- [`processed_sales_data.csv`](processed_sales_data.csv): CSV file containing preprocessed sales data.
- [`sales_data.csv`](sales_data.csv): Raw sales data CSV file.
- `README.md`: This file, providing an overview of the repository.

## Data Files

### [`sales_data.csv`](sales_data.csv)

This file contains the raw sales data with the following columns:
- `Business Unit`
- `PH1`
- `PH2`
- `Item Code`
- `Item Description`
- `Sales Channel`
- `Month`
- `Year`
- `Stat Forecast`
- `Actual Amount`

### [`processed_sales_data.csv`](processed_sales_data.csv)

This file contains the preprocessed sales data with the following columns:
- `Business Unit`
- `PH1`
- `PH2`
- `Item Code`
- `Item Description`
- `Sales Channel`
- `Stat Forecast`
- `Actual Amount`
- `Date`

### [`priority_data_fixed.csv`](priority_data_fixed.csv)

This file contains the prioritized sales data with the following columns:
- `Business Unit`
- `PH1`
- `PH2`
- `Item Code`
- `Item Description`
- `Sales Channel`
- `Stat Forecast`
- `Actual Amount`
- `Date`
- `Deviation`
- `Deviation Category`
- `Priority`

## Notebooks

### [`analysis.ipynb`](analysis.ipynb)

This notebook performs the following tasks:
1. **Data Loading**: Loads the raw sales data from [`sales_data.csv`](sales_data.csv).
2. **Data Preprocessing**: Converts date columns, cleans numeric columns, and saves the processed data to [`processed_sales_data.csv`](processed_sales_data.csv).
3. **Time Series Decomposition**: Aggregates data by item description and date, and performs time series decomposition on the actual amounts.
4. **Deviation Calculation**: Calculates deviations between forecast and actual amounts, classifies deviations into categories, and assigns priorities.
5. **Saving Priority Data**: Saves the prioritized data to [`priority_data_fixed.csv`](priority_data_fixed.csv).

### [`Charts.ipynb`](Charts.ipynb)

This notebook generates various visualizations based on the processed and prioritized data:
1. **Forecast vs Actual Amount Over Time**: Line plots for the first 5 items.
2. **Deviation Distribution**: Histogram of deviations.
3. **Deviation Category Breakdown**: Pie chart of deviation categories.
4. **Priority-Based Exception Analysis**: Count plot of priorities.
5. **Category-Level Performance**: Bar plot of deviation sums by category.
6. **Forecast Accuracy Over Time**: Line plot of average forecast error over time.
7. **Deviation Trend by Item Description**: Line plots and subplots for deviation trends by item description.
8. **Deviation by Deviation Category**: Boxplot of deviations by category.
9. **Correlation Heatmap**: Heatmap of correlations between numerical columns.
10. **Deviation by Year**: Bar plot of total deviation by year.
11. **Monthly Forecast Error Trend**: Line plot of average forecast error by month.
12. **Deviation Over Time for Specific Items**: Scatter plot of deviations over time for specific items.
13. **Deviation Category by Sales Channel**: Count plot of deviation categories by sales channel.
14. **Deviation Distribution by Item Description**: Boxplot of deviations by item description.
15. **Top 10 Items with Highest Average Deviation**: Boxplot of deviations for top 10 items.
16. **Total Deviation by Product Item**: Bar plot of total deviation by product item.
17. **Historical Forecast vs Actuals for Top Items**: Subplots of forecast vs actual amounts for top items.

