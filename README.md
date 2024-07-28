# IMDb Movies Dashboard (General Analysis)

## Project Overview

This project aims to create a comprehensive dashboard for analyzing IMDb movie data. The dashboard provides insights into various aspects of movies, such as profitability, ratings, and filmmaking expenditures across different countries. The analysis is presented through four key visualizations:

1. **Top 10 Movies by Profit**
2. **Top 10 Countries by Filmmaking Expenditure**
3. **Top 10 Directors by IMDb Rating**
4. **Top 10 Movies by IMDb Rating**

## Data Preprocessing

### Currency Standardization

One of the primary challenges was the inconsistency in currency representation for budget and gross revenue columns (`budget_us_dollar` and `gross_us_dollar`). To address this, the following steps were undertaken:

- **Country Identification**: Identified the country for each movie in the dataset.
- **Currency Conversion**: Created a mapping table for countries and their respective currencies. Converted all budget and gross revenue figures to USD based on the country-specific currency to ensure uniformity.
- **Profit Calculation**: Computed the profit for each movie as the difference between gross revenue and budget, both standardized in USD.

### Data Cleaning

- **Movie Titles**: Cleaned the `movie_title` column by removing any extraneous characters, such as "Â ".
- **Genres**: Simplified the `genres` column by selecting the first listed genre as the primary genre for classification purposes.

## Visualization

### Pivot Tables

Four pivot tables were created to generate the visualizations for the dashboard:

1. **Most 10 Movies by Profit**: Displayed the top 10 movies based on their profit margins.
2. **Most 10 Countries Spending on Filmmaking**: Illustrated the top 10 countries by their filmmaking expenditures.
3. **Top 10 Directors by IMDb Rating**: Showcased the directors with the highest average IMDb ratings.
4. **Top 10 Movies by IMDb Rating**: Highlighted the top 10 movies based on IMDb ratings.

### Charts

The visualizations were created using the following types of charts:

- **Bar Charts**: Used for displaying the top 10 movies by profit and top 10 directors by IMDb rating.
- **Pie Chart**: Used for showing the most 10 countries by filmmaking expenditures.
- **Column Chart**: Used for presenting the top 10 movies by IMDb rating.

![IMDB Movies Dashboard ](https://github.com/user-attachments/assets/330216c7-6a52-4fe0-ae48-cbe4e6d02c62)

## Insights

- **Profitability**: The chart reveals which movies have generated the highest profits, providing insights into successful genres and production strategies.
- **Filmmaking Expenditure**: The pie chart offers a clear picture of which countries invest the most in filmmaking, indicating the global distribution of the film industry.
- **Director Performance**: The bar chart of top directors highlights which directors are most favored by audiences based on IMDb ratings.
- **Movie Ratings**: The column chart of top-rated movies showcases audience preferences and high-performing films.

## Conclusion

The IMDb Movies Dashboard provides valuable insights into the film industry, allowing for data-driven decision-making and strategic planning. By standardizing currency data, cleaning movie titles, and simplifying genre classification, we ensure the accuracy and usability of the data. The visualizations offer a clear and concise representation of key metrics in the movie industry.

## Future Work

- **Expand Data Sources**: Incorporate additional data sources to provide a more comprehensive analysis.
- **Advanced Analytics**: Implement more advanced analytical techniques, such as machine learning, to predict movie success.
- **Interactive Dashboard**: Develop an interactive version of the dashboard for real-time data exploration.

