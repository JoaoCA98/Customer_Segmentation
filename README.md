# Hotel Customer Segmentation Project
[Dataset] | [Notebook](https://github.com/JoaoCA98/Customer_Segmentation/blob/main/Clustering_Customer_Segmentation.ipynb)
## Introduction
In today's competitive business environment, understanding customer behavior is crucial. To effectively target and engage customers, organizations must move beyond traditional market segmentation and adopt data-driven approaches. This project revolves around creating an up-to-date customer segmentation strategy for Hotel H, a member of the independent hotel chain C in Lisbon, Portugal. By harnessing customer data, the aim is to redefine how customers are grouped for personalized marketing efforts.

## Customer Segmentation in Hotel H
Hotel chain C, including Hotel H, relied on a conventional market segmentation based solely on the origin of customers. However, the marketing manager, A, recognized the limitations of this approach. The existing segmentation failed to account for vital factors such as demographics, behavior, and geographic origin. A realized the importance of refining this segmentation to create effective marketing strategies, especially considering the diverse distribution channels utilized by modern hotels.

## The Challenge
The challenge posed by A is to transition from traditional segmentation methods to a modern, data-driven approach based on Hotel H's customer database.

## Business Understanding
### Background and Business Objectives
This project adhered to the Crisp-DM Project Lifecycle, encompassing Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation & Deployment phases. The objective was to ensure data quality and create an effective segmentation model.

Python libraries used:
- Pandas: Data Analysis
- NumPy: Mathematical operations
- Matplotlib: Data visualization
- Seaborn: Statistical data visualization
- Sklearn: Scaling, normalization, pairwise distances
- Category_encoders: Categorical variable encoding techniques

## Data Understanding Summary
The dataset comprises 83,590 observations with 31 features, including 5 categorical and 26 numerical variables. Highlights from data exploration:
- Categorical variables like Nationality, Distribution Channel, Market Segment, etc., won't be used for clustering as K-Means is inappropriate for categorical data.
- Age contains outliers (max value: 122) and needs further investigation.
- AverageLeadTime includes negative values and varying means and medians, indicating outliers.
- LodgingRevenue and OtherRevenue likely have outliers in the positive direction.
- BookingsChedIn shows a wide range of days (max: 66), warranting further investigation.
- PersonsNights and RoomNights are negatively skewed with high max values.

## Data Preparation
Data preparation involved:
1. Creating copies of the original dataset.
2. Addressing missing values, outliers, and skewed distributions.

## Insights
- Cluster 0: Asian and American corporate and aviation clients who book directly with the hotel.
- Cluster 1: Leisure-seeking tourists, mainly from Africa and Europe.
- Cluster 2: Classic Group Tourists, booking through travel agent operators, mostly for group trips.
- Cluster 3: High spenders, primarily from Oceania, prefer high floors and luxurious amenities.
- Cluster 4: Corporate Complimentary Bookings, predominant in corporate bookings.

## Conclusion
This project highlighted the importance of data-driven customer segmentation for effective marketing strategies. The data preparation phase revealed biases and challenges in the dataset. The identified clusters provide valuable insights for Hotel H's marketing efforts, enabling them to tailor strategies based on customer behavior and preferences.
