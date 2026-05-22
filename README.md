# Amazon Sales Analysis

This project analyzes an Amazon sales dataset containing product prices, discounts, ratings, rating counts, reviews, and product categories. The goal is to explore customer behavior and understand how pricing, discounts, and categories are related to product ratings and review activity.

## Project Overview

This is an exploratory data analysis project using Python. The analysis focuses on over 1,000 Amazon products and investigates whether higher discounts lead to better ratings, which categories perform best, and which categories receive the most customer reviews.

The project includes data cleaning, feature engineering, correlation analysis, grouped summaries, and data visualization.

## Research Questions

This project answers the following research questions:

1. Does a higher discount percentage lead to higher product ratings?
2. Which product categories have the highest average ratings?
3. Are heavily discounted products more likely to receive customer reviews?
4. What is the relationship between actual price and customer ratings?
5. Which product categories receive the most customer reviews based on rating count?

## Dataset

The dataset includes Amazon product information such as:

- Product name
- Product category
- Discounted price
- Actual price
- Discount percentage
- Rating
- Rating count
- Review information
- Product links

The dataset was loaded from a Kaggle Amazon sales dataset.

## Data Cleaning

Several columns were cleaned and converted into numeric format for analysis:

- Removed currency symbols and commas from price columns
- Converted `discounted_price` and `actual_price` to numeric values
- Removed `%` from `discount_percentage`
- Converted `rating` and `rating_count` to numeric values
- Created a new `main_category` column from the original category column
- Created discount groups for grouped comparison

## Analysis and Visualizations

The project includes visualizations such as:

- Scatter plot of discount percentage vs. rating
- Bar chart of average rating by main category
- Bar chart of average rating count by discount group
- Scatter plot of actual price vs. rating
- Log-scale scatter plot of actual price vs. rating
- Bar chart of total rating count by category
- Distribution of product ratings
- Distribution of discount percentages

## Key Findings

- Product ratings are mostly concentrated between 3.8 and 4.5.
- Higher discounts do not clearly lead to higher product ratings.
- Some categories, such as OfficeProducts, Toys&Games, and HomeImprovement, show higher average ratings.
- Actual price has only a weak relationship with customer rating.
- Electronics receives the highest total number of customer reviews.
- Rating count can be used as an indicator of product popularity and customer engagement.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Kaggle dataset

## Project Files

```text
Amazon_Sales_Dataset2.ipynb   # Main notebook for data cleaning, analysis, and visualization
README.md                     # Project documentation