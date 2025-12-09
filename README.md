# Campsite Reservation Analysis

## Question

**What are the best times of year to book a campsite and what is the typical lead time required?**

## Project Overview

This project analyzes campsite reservation patterns using data from recreation.gov to help campers understand optimal booking lead times and campsite popularity. With popular campsites becoming increasingly difficult to book, this analysis provides data-driven insights into when to book and how far in advance to plan.

## Data Source

The analysis uses several years of historical reservation data from **recreation.gov**, the primary platform for booking campsites across the United States. The dataset includes:

- Reservation dates (booking date and arrival date)
- Park/campsite information
- Stay duration and party size
- Geographic location data

**Current Dataset**: `data/reservations_2024_california_sample.csv`

## Analysis and Predictions

### 1. Data Analysis Techniques

#### Decision Tree Regression
- **Purpose**: Demand and occupancy forecasting
- **Rationale**: Decision Trees effectively capture non-linear, time-based patterns in seasonal camping demand
- **Features**: Month, day of week, quarter, weekend indicators, seasonal flags, park popularity, and historical lead times

#### K-means Clustering
- **Purpose**: Customer behavior segmentation
- **Rationale**: Identifies distinct camper segments based on booking patterns, which affects occupancy forecasting
- **Features**: Lead time patterns, stay duration, group size, booking volume, and planning consistency

### 2. Exploratory Data Analysis
- Lead time distribution analysis
- Monthly reservation patterns
- Booking timeline heatmaps
- Park popularity rankings
- Percentile-based booking insights

## Expected Results

1. **Optimal Booking Times**: Clear identification of peak and off-peak seasons for campsite reservations
2. **Lead Time Recommendations**: Data-driven guidance on how far in advance to book for different times of year
3. **Customer Segments**: Understanding of different camper behavior patterns and their impact on availability
4. **Park-Specific Insights**: Demand patterns for the most popular state parks

### Future Enhancements
- Geolocation-based filtering to provide region-specific recommendations
- Predictive booking difficulty scores for specific parks and dates
- Real-time availability integration

## Why This Matters

**Booking popular campsites has become increasingly difficult**, with many sites filling up within minutes of becoming available. This analysis addresses a critical need for campers by:

- Providing strategic booking guidance based on historical data
- Helping families and outdoor enthusiasts plan vacations more effectively
- Reducing frustration and improving success rates for securing reservations
- Democratizing access to camping through better information

## License

This project is for educational and research purposes.

## Acknowledgments

Data sourced from recreation.gov, the official recreation resource for federal lands.
