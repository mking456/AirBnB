![airbnb](https://github.com/mking456/AirBnB/blob/main/New-York-City-Brooklyn-Bridge-Panorama-Juergen-Roth-2.jpg)

# New York Airbnb Listings Analysis

## Project Overview
This project aims to analyze Airbnb listings in New York City, focusing on room types, prices, and availability across different neighborhoods. The analysis uncovers host behavior, pricing patterns, and potential outliers in the dataset. Additionally, actionable insights and recommendations are provided for both guests and hosts.

## Dataset
The dataset consists of 20,765 entries and 22 features. Some of the key columns include:
- `id`: Unique identifier for each listing
- `name`: Title of the listing
- `host_name`: Name of the host
- `neighborhood_group`: Borough where the listing is located
- `latitude` / `longitude`: Geolocation of the listing
- `price`: Nightly rental price
- `room_type`: Type of accommodation (e.g., entire home, private room)
- `reviews_per_month`: Average monthly reviews for the listing
- `availability_365`: Number of available days in the year

## Steps and Workflow

### 1. Data Cleaning
- **Handle missing data**: Missing values were found in `price`, `neighborhood`, and `beds` columns and were handled accordingly.
- **Fix data types**: The `last_review` column was converted into a datetime object.
- **Remove outliers**: Listings with prices greater than $1,000 were capped to avoid skewed visualizations.

### 2. Exploratory Data Analysis (EDA)
- **Room Type Distribution**: 
  - Visualized room types using bar plots.
  - Found that "Entire home/apt" is the most common room type.
- **Neighborhood Group Insights**: 
  - Analyzed price variations across boroughs, finding Manhattan has the highest average prices.
- **Availability Trends**: 
  - Used heatmaps to show correlations between price, availability, number of reviews, and beds.
- **Price Distribution**: 
  - Histograms revealed that most listings fall within a price range of $50 to $300.
- **Host Listings**: 
  - Analyzed hosts with multiple listings using box plots.
- **Review Behavior**: 
  - Used pair plots to show relationships between number of reviews, price, and availability.

### 3. Data Visualization
- **Pairplot**: Correlations among price, availability, and number of reviews.
- **Heatmap**: Visualized correlations among numerical features.
- **Histograms and Boxplots**: Used to detect price outliers.
- **Bar Charts**: Displayed distributions of room types and neighborhood groups.

## Key Findings and Insights

- **Price Trends**: 
  - Manhattan has the most expensive listings, followed by Brooklyn.
  - Entire homes/apartments are significantly more expensive than private or shared rooms.
- **Room Type Distribution**: 
  - Entire homes/apartments are the most common type, but private rooms offer more budget-friendly options.
- **Outliers in Price**: 
  - Detected a few listings priced at $10,000+, indicating the need to filter extreme values.
- **Availability Patterns**: 
  - Listings with high availability tend to have lower prices and more reviews, likely due to better guest experiences.
- **Host Behavior**: 
  - Some hosts manage multiple listings, indicating a trend towards professional hosting.

### Recommendations
- **For Guests:
Look for listings with high availability and good reviews for a better experience.
Private rooms in Brooklyn offer more affordable stays compared to Manhattan.
- **For Hosts:
Improve availability and respond to reviews promptly to attract more bookings.
Manage pricing effectively to compete within your borough's market.
### Future Work
Price Prediction: Use machine learning to predict listing prices based on room type, location, and other features.
Sentiment Analysis: Perform sentiment analysis on guest reviews to better understand guest experiences.
Interactive Dashboard: Create an interactive dashboard using Plotly or Tableau for live data visualization and monitoring.
### Conclusion
This analysis of New York's Airbnb listings provides valuable insights for both guests and hosts. Future work may involve advanced analytics, predictive modeling, and interactive data visualizations to further enhance the findings.
