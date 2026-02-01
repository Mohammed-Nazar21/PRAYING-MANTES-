Programming Assignment
⚡ Electricity Consumption and Cost Analysis
👥 Group Information
Group Name: PRAYING MANTES 
Course: SKEE 1033 – Scientific Programming 
Section: 17 
Lecturer: Assoc. Prof. Muhammad Mun`im Ahmad Zabidi 
Group Members:- Ziad Hany Farouk Sadek Askar – A25KE0046- Mohammed Nazer – A25KE4023- Judy Ahmed Salah Elzaabalawy – A25KE0049- Mazin B. S. Fayyad – A25KE0441- Abubakr Atif Mohamed Abdelmalik – A25KE4005
 Project Introduction
This report documents the implementation and analysis of the Electricity Consumption and Cost
Analysis project developed for the SKEE 1033 Scientific Programming course. The complete
implementation (dataset handling, analysis workflow, and modelling scripts) is maintained in the
group’s GitHub repository and was executed using Google Colab for reproducibility and transparency.
The primary objective of the project is to analyze household electricity consumption patterns across
Urban, Suburban, and Rural regions from 2018 to 2022, and to investigate how household
occupancy influences electricity usage and cost. Beyond descriptive statistics, the project applies
predictive modelling to estimate electricity costs based on real-world variables
Dataset Overview
The dataset consists of monthly household electricity records with the following characteristics:

Time Period: 2018 – 2022 
Regions Covered: Urban, Suburban, Rural 
Main Variables:
Consumption_kWh : Monthly electricity usage 
Cost_RM : Monthly electricity cost (calculated using RM 0.57 per kWh) 
Occupants : Number of people living in the household
Dataset Overview
The dataset consists of monthly household electricity records with the following characteristics:

Time Period: 2018 – 2022 
Regions Covered: Urban, Suburban, Rural 
Main Variables:
Consumption_kWh : Monthly electricity usage 
Cost_RM : Monthly electricity cost (calculated using RM 0.57 per kWh) 
Occupants : Number of people living in the household
 Task 2: Exploratory Data Analysis (NumPy & Pandas)
Objective: Identify patterns and validate relationships between variables.

Descriptive Statistics:
Mean, median, and standard deviation of electricity consumption were calculated for each
region to establish baseline behavior.
Correlation Analysis:
Pearson correlation was used to measure the relationship between household size and
electricity usage, supporting the inclusion of occupant count as a key predictive feature
 Task 3: Data Visualization (Matplotlib)
Objective: Reveal trends and comparisons through graphical analysis.
Line Plots: Displayed monthly consumption trends across the five-year period. 
Multi-Line Charts: Compared electricity usage between Urban, Suburban, and Rural regions. 
Scatter and Box Plots: Illustrated the relationship between number of occupants and electricity
consumption.
 Key Results and Observations
️
Regional Consumption Trends
Seasonal Behavior:
Electricity usage peaks consistently between March and May, coinciding with higher
temperatures and increased air-conditioning use.
The lowest consumption is observed from September to November, likely due to milder
weather conditionsRegional Comparison:
 
Urban households: Highest usage (approximately 450–550 kWh) 
Suburban households: Moderate usage (350–470 kWh) 
Rural households: Lowest usage (250–370 kWh)
Year-to-Year Stability:
Consumption patterns remain relatively stable across all years, indicating strong dependence on
seasonal and environmental factors rather than behavioral change.
Occupancy vs Consumption Relationship

Unexpected Trend:
Analysis shows a negative correlation between household size and total electricity
consumption.
Key Observation:
Smaller households (1–2 occupants) often exceed 500 kWh monthly usage. 
Larger households (6–7 occupants) commonly remain below 300 kWh.
Interpretation:
This pattern suggests socioeconomic and lifestyle influences. Larger families in the dataset are
more likely to live in rural or landed homes with less dependence on air-conditioning, while
smaller households often reside in urban apartments with high cooling demand. As household
size increases, electricity consumption per person decreases, indicating more efficient shared
usage.
Task 4: Predictive Modelling (Scikit-Learn)
Objective: Estimate monthly electricity cost using machine learning.
Model Used: Linear Regression 
Rationale: Electricity cost is directly proportional to energy consumption, making linear
regression suitable.
Data Split: 80% training, 20% testing
Input Features:
Number of occupants 
Month 
Region
Target Variable:
Electricity cost (RM)
 Predictive Performance and Interpretation

The regression model smooths out random fluctuations observed in raw data. 
Predicted trends successfully capture:
Seasonal consumption patterns 
Average increase in usage with occupancy
Although individual outliers cannot be perfectly predicted, the model achieves a high R² value,
confirming strong reliability for baseline forecasting. Occupancy and month emerge as the most
influential predictors
 Cognitive Interpretation of Patterns

Pandemic Influence (2020–2022):
Increased electricity usage during these years aligns with COVID-19 Movement Control Orders
(MCO), where remote learning and work significantly raised daytime energy demand.
Seasonal Peaks:
Higher consumption aligns with Malaysia’s tropical climate, driven by heatwaves and monsoon
seasons that keep residents indoors.
Urban–Rural Gap:
Urban households show higher predicted consumption due to greater access to energy
intensive appliances such as multiple air conditioners, dryers, and electronic devices
 Prescriptive Insights and Recommendations
High-Occupancy Residences:
Homes with more than five occupants should be prioritized for energy audits and smart meter
installations to monitor and reduce inefficiencies.
Seasonal Demand Management:
Utility providers could introduce Time-of-Use (ToU) tariffs during peak months to encourage off
peak energy usage.
Future Housing Design:
With hybrid work and study patterns becoming permanent, new housing developments should
emphasize passive cooling, insulation, and natural ventilation to reduce air-conditioning
dependence.
