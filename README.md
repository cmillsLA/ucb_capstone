### Campsite Reservation Analysis

#### Executive Summary

This project analyzes California campsite reservation patterns using data from Recreation.gov to provide insights for optimizing campsite bookings. Using machine learning techniques I developed a comprehensive system that forecasts demand, segments customer behavior, and recommends campsites through a natural language interface.

Users can interact with historical data to plan their trip or find similar alternatives to popular campsites.  This recommendation system helps users understand optimal booking windows, discover alternative parks, and receive instant answers to natural language queries like "What campsites are available for last minute trips?" This addresses the critical problem of popular campsites filling within minutes of availability, improving booking success rates for families and outdoor enthusiasts.

#### Rationale
Given the limitations of the Recration.gov website, it can be very time consuming to find available campsites.  This is especially true during peak season or for popular campsites.  This recommendation system will help users find alternative campsites or understand the appropriate lead time to book a site that is more popular.  In addition, this can be used to find campsites that are likely to be available for a last minute weekend trip.

#### Research Question
This research addresses three key questions:
1. How far in advance do campers typically book reservations for different seasons?
2. Which parks and time periods have the highest demand and longest lead times?
3. Can we predict optimal booking windows and recommend alternative campsites based on historical patterns?

#### Data Sources
Data sourced from <a href="https://recreation.gov">recreation.gov</a>, the official recreation resource for federal lands.

#### Methodology
This analysis employs a multi-faceted approach combining exploratory data analysis, machine learning, and recommender systems:

**1.  Exploratory Data Analysis & Visualization:**
- Lead time distribution analysis and percentile calculations
- Seasonal booking pattern identification
- Booking month vs. arrival month heatmaps
- Park popularity rankings and demand trends

**2. Predictive Modeling**
- Decision Tree Regression: Baseline model for demand forecasting using temporal features (month, day of week, quarter, seasonal indicators)
- Gradient Boosting: Enhanced model leveraging gradient descent optimization for improved prediction accuracy
- K-means Clustering: Customer segmentation to identify distinct booking behavior patterns (last-minute bookers, planners, weekend campers)

**3. Recommendation Systems**
- Item-Based Collaborative Filtering: Identifies similar parks based on shared booking patterns
- User-Based Collaborative Filtering: Recommends parks based on similar user profiles (booking timing, duration, planning horizon)
- Natural Language Query Interface: Allows users to ask questions in plain English about availability, lead times, and recommendations

**4. Model Evaluation**
- R² scores and mean squared error for predictive models
- Silhouette scores for clustering quality
- Cosine similarity metrics for recommendation accuracy

#### Results
- **Peak booking periods** occur during summer months (June-August), requiring significantly longer lead times (90+ days)
- **Customer segmentation** revealed distinct camper profiles: last-minute bookers, weekend warriors, and advance planners
- **Recommendation system** successfully identifies similar parks and provides personalized suggestions based on booking patterns

#### Next steps
- **Direct linking to campsite** allow users to visit the campsite booking url directly from the recommendation results
- **Geolocation** when searching for similar campsites, use the geolocation of the campsite identified in the user input

#### Outline of project
- **<a href="index.ipynb">Load the data, vizualizations</a>**
- **<a href="recommendations.ipynb">View the recommendations</a>**

#### License

This project is for educational and research purposes.
