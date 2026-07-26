# Sales Data Exploratory Data Analysis

This project explores a retail sales dataset using Python, Pandas, Matplotlib, and Seaborn to understand revenue patterns, customer behaviour, and transaction characteristics.

## Project overview

The analysis is built around a cleaned dataset called `clean_sales_data.csv`, which is loaded with `transaction_id` as the index and `date` parsed as a datetime field. The notebook investigates overall sales performance, transaction value distribution, customer segments by gender and age, and time-based revenue trends, supported by multiple saved charts such as `monthly_sales.png`, `revenue_by_day.png`, `revenue_by_month.png`, and age-related visualisations.

## Dataset

The project uses both the raw file `sales_data.csv` and the cleaned file `clean_sales_data.csv`. The cleaned dataset includes the columns `date`, `customer_id`, `gender`, `age`, `product_category`, `quantity`, `price_per_unit`, and `total_amount`, with `transaction_id` used as the row index.

## Key findings

- Total revenue in the dataset is 456,000 across 1,000 transactions.
- The average transaction value is 456.0, with a median of 135, an interquartile range from 60 to 900, and a maximum observed transaction value of 2,000.
- Transaction values are right-skewed, which suggests that most purchases are relatively small while a smaller number of large orders contribute heavily to revenue.
- Average order value is almost identical by gender: 456.55 for female customers and 455.43 for male customers.
- Average order value declines across age bands, from 500.30 for customers aged 18–25 to 412.36 for customers aged 56+.

## Visualisations

The project includes several saved figures that support the EDA:

- `kde_plot_transaction_value.png` for transaction value distribution.
- `monthly_sales.png`, `revenue_by_day.png`, and `revenue_by_month.png` for time-based revenue analysis.
- `age_distribution_by_gender.png` and `age_distribution_by_product.png` for customer demographic exploration.
- `price_vs_quantity_by_product_category.png` and `revenue_share_by_age_band.png` for product and segment-level insights.

## Tools and libraries

The notebook environment uses Python with Pandas, Matplotlib, and Seaborn. The project also creates an `images/charts` directory for outputs generated during the analysis.

## Project structure

```text
python project/
├── sales data analysis.ipynb
├── data cleaning process.ipynb
├── sales_data.csv
├── clean_sales_data.csv
├── kde_plot_transaction_value.png
├── monthly_sales.png
├── revenue_by_day.png
├── revenue_by_month.png
├── age_distribution_by_gender.png
├── age_distribution_by_product.png
├── price_vs_quantity_by_product_category.png
├── revenue_share_by_age_band.png
└── images/
```

## Example questions answered

This EDA helps answer questions such as:

- How much total revenue does the business generate?
- What does the distribution of transaction values look like?
- Does average order value differ by gender?
- Which age groups contribute higher-value purchases?
- How does revenue change over time?

## How to run

1. Open the notebooks in Jupyter Notebook or JupyterLab.
2. Install the required libraries, including Seaborn, Pandas, and Matplotlib.
3. Run the data cleaning notebook first if the cleaned dataset needs to be regenerated.
4. Run `sales data analysis.ipynb` to reproduce the analysis and charts.

## Future improvements

Possible next steps for the project include adding product-category level KPIs, identifying seasonal trends more explicitly, and building an interactive dashboard version of the analysis from the cleaned dataset.
