# Superstore Sales & Profit Analysis

Analysis of 9,994 retail orders (2014-2017) to find what drives sales and profit, and where the business is losing money.

## Dataset
Kaggle: Sample Superstore (`Sample_Superstore.csv`), 9,994 orders, 21 columns after feature engineering. No missing values or duplicates.

## Steps
1. **Cleaning:** converted mixed-format date columns, validated ship dates, created Year, Month, Ship Days and Profit Margin columns.
2. **EDA:** sales and profit by year, category, sub-category and region.
3. **Discount analysis:** compared profit across discount bands, then drilled into the worst sub-category and region.

## Key Insights
- Sales grew 51% (USD 484K to 733K) and profit grew 89% (USD 49.5K to 93.4K) from 2014 to 2017. Overall margin is 12.5%.
- Furniture earns only a 2.5% margin on USD 742K sales, versus about 17% for Office Supplies and Technology.
- Tables (-USD 17.7K), Bookcases (-USD 3.5K) and Supplies (-USD 1.2K) are loss-making sub-categories.
- Orders with a discount above 20% (1,393 orders, 14% of total) lost USD 135.4K combined, equal to about 47% of total profit.
- Tables earned USD 13.3K with no discount but lost money at every higher discount band, which suggests discounting, not the product itself, drives the loss.
- Central region has the highest average discount (24.0%) and the lowest margin (7.9%).

## Recommendation
Cap discounts at 20%, especially for Furniture and in the Central region.

## Limitations
This is observational data, so the link between discount and loss is a strong association and not proof of cause.

## Tools
Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook
