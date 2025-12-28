# Amazon E-Commerce Sales Analysis
This project focuses on cleaning and analyzing a dataset of ~50,000 Amazon retail transactions to uncover sales trends, fulfillment efficiency, and customer purchasing patterns.

## 📊 Project Overview
The primary goal of this analysis is to transform raw e-commerce data into actionable business insights. The project is split into two main phases:

1. **Data Cleanup**: Handling missing values, correcting data types (especially dates), and removing redundant columns to prepare a "gold" dataset.

2. **Exploratory Data Analysis (EDA)**: Visualizing Key Performance Indicators (KPIs) such as total revenue, unit sales, and fulfillment status distributions.

## 🛠️ Tech Stack
- **Language**: Python

- **Libraries**: Pandas, NumPy, Matplotlib (using fivethirtyeight style), KaggleHub

- **Environment**: Jupyter Notebook / Google Colab

## 🧹 Data Cleaning Highlights
The cleaning process involved several critical steps to ensure data integrity:

- **Date Standardization**: Converted date strings into datetime64 objects for time-series analysis.

- **Dimensionality Reduction**: Dropped columns with single unique values (e.g., sales_channel, ship_country) and redundant index columns.

- **Handling Nulls**: Identified and managed missing values in fields like promotion_ids and amount.

- **Custom Formatters**: Developed a helper function to format currency into the Indian Rupee (INR) numbering system (e.g., Lakhs and Crores).

## 📈 Key Insights from EDA
The analysis tracked several Global KPIs:

- **Revenue Tracking**: Total revenue and units sold across different product categories.

- **Fulfillment Analysis**: Comparison of Amazon-fulfilled vs. Merchant-fulfilled orders.

- **Order Status**: Detailed breakdown of order statuses, including shipped, cancelled, and pending.

- **Note**: Amazon-fulfilled orders primarily show 'shipped', 'cancelled', and 'pending' statuses.

## 📁 Project Structure
- `amazon_data_cleanup.ipynb`: Initial ingestion and rigorous cleaning of the raw CSV file.
- `Amazon_detailed_Eda.ipynb`: In-depth visualization and KPI calculation from the cleaned data.

## 🚀 How to Run
1. Clone the repository.

2. Install dependencies:

```
pip install pandas matplotlib numpy kagglehub
```

3. Run the notebooks: Start with the cleanup notebook to generate the processed dataset, followed by the EDA notebook for insights.
