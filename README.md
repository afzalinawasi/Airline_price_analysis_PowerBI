# Airline price analysis-PowerBI
Power BI dashboard analyzing airline ticket pricing across booking window, routes, airlines, and travel class. The project highlights key pricing drivers using median-based KPIs, ensuring accurate comparisons while handling class imbalance and skewed distributions.
## Overview
This project analyzes airline ticket pricing patterns using Power BI, focusing on how prices vary across factors such as booking window, airline, route, stops, and travel class (Economy vs Business).
The goal is to provide actionable insights for pricing strategy and customer decision-making through an interactive dashboard.
### Executive summary 
1. Airline ticket prices are primarily influenced by booking timing, route characteristics, airline choice, and travel class, with the booking window showing the largest observable variation (~2.5–3x).
2. Prices increase sharply in the final 1–2 days before departure, while booking 15–30 days in advance offers the lowest fares.
3. For airlines offering both classes, Business fares are several times higher than Economy (~5x–9x range), reflecting strong premium segmentation.
4. Airline selection can lead to up to ~2x price difference, indicating meaningful brand and service positioning.
5. Pricing is highly skewed, with most tickets in lower ranges (₹3K–₹10K) and a small number of high-value fares driving variability.

_Note: All insights are correlational, as key variables such as distance, demand, and seasonality are not available in the dataset._ 
## Objective
The analysis aims to answer the following key questions:
Does ticket price vary across airlines?
How does last-minute booking impact price?
Does departure/arrival time influence pricing?
How do routes (source–destination) affect price?
What is the price difference between Economy and Business class?
## Methodology
### Data cleaning:
No missing or duplicate records found
Standardized categorical values
Feature engineering:
Created Booking Window (Days Left)
### Data Considerations
- Not all airlines offer Business class
→ Class-based KPIs are calculated only for valid airline-class combinations
- Dataset does not include: Distance, Demand, and Seasonality
👉 Therefore, all insights are correlational, not causal
### Metric selection:
- Used Median instead of Average to handle skewed price distribution
## Analysis approach:
1. Visual trend analysis (not statistical modeling)
2. Structured into “What” vs “Why” dashboards
## The Power BI solution is divided into two dashboards:
### 1. Pricing Landscape (What is happening)
Median price KPIs (Economy & Business)
Airline-wise price comparison
Route-based price heatmap
Time-based pricing patterns
Price distribution
### 2. Price Drivers (Why it is happening)
Booking window impact (days left vs price)
Stops vs price relationship
Class-based pricing comparison
Trend analysis of booking behavior
## Key insights
1. Booking window is the strongest pricing driver
→ Median prices rise from ~₹4.5K (30+ days) to ~₹13.6K (1–2 days), a ~3x increase
2. Business class fares show strong premium segmentation
→ ~9x higher than Economy (only for airlines offering both classes)
3. Airline choice significantly impacts pricing
→ Median fares range from ~₹3.3K to ~₹6.5K (~2x variation)
4. Route-based pricing variability is high
→ Certain routes show consistently higher fares, indicating demand-supply imbalance
5. Stops are not a direct pricing driver
→ Higher prices are associated with more stops due to route complexity
6. Time of departure/arrival has limited influence
→ Only ~10–15% variation compared to booking window impact
## Recommendations
### 1. Business or Pricing strategy
1. Leverage dynamic pricing for last-minute bookings
2. Optimize pricing at the route level based on demand patterns
3. Maintain competitive pricing in the economy segment due to high price sensitivity
4. Leverage class segmentation to target premium vs budget customers
### 2. Customer strategy
1. Book flights 15–30 days in advance for the best prices
2. Avoid last-minute bookings due to steep price increases
3. Compare airlines for the same route, as price differences of up to ~2x exist across carriers → Opt for direct flights when cost-sensitive
