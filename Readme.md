# Patients Emergency Room Visit Report

![Dashboard](/dash.png)

## Introduction
This report presents a detailed analysis of emergency room visits.  
The goal is to understand patient demographics, visit behavior, referral sources, and satisfaction levels.  
The analysis focuses on service utilization, patient wait times, and departmental referrals.  
Power BI was used end to end for data preparation, modeling, analysis, and visualization.  

## About the Data
The dataset contains structured emergency room records.  
It includes information on patient demographics, age groups, referral status, gender, race, appointment types, satisfaction scores, and visit frequency.  
The records span two years, covering both weekdays and weekends.  

## Methodology

### Data Collection
Data was sourced directly from hospital emergency room systems.  
The dataset included both administrative and non-administrative appointments.  
Information on referrals by department was captured, along with yearly and monthly visit counts.  

### Data Cleaning and Transformation
All cleaning, transformation, and preparation were performed in Power BI.  
Appointment types were split into two categories, administrative and non-administrative.  
Nulls were handled for gender and race.  
Outliers in wait time were normalized to prevent skewing results.  
Age groups were defined as Infant, Early Childhood, Middle Childhood, Teenager, and Adult.  

### Exploratory Data Analysis
Exploration was conducted in Power BI using measures and DAX queries.  
Trends were studied across age groups, week type, year, gender, and race.  
Heatmaps were generated to measure average wait times by race and age group.  
Time-based patterns were explored to identify weekday vs weekend demand.  

### Visualization
Power BI dashboards were designed to present results in a clear, interactive way.  
Charts include line charts for yearly trends, bar charts for referrals, and heatmaps for satisfaction vs wait times.  
Visuals were linked with slicers to allow filtering by variables such as wait time, referral type, and patient demographics.  

### Statistical Analysis
All descriptive statistics were calculated in Power BI.  
- Total patient visits: 9,216  
- Administrative appointments: 50.04%  
- Non-administrative appointments: 49.96%  
- Average satisfaction score: 5.47  
- Average wait time: 35.26 minutes  
- Services not rated: 75.1%  
- Referral split: 41.41% referred, 58.59% unreferred  

### Interpretation and Recommendations
Key insights suggest adults represent the largest share of visits.  
Referrals are concentrated in General Practice and Orthopedics.  
Satisfaction levels are linked to reduced wait times, especially among younger patients.  
The high percentage of unrated services is a gap in patient feedback collection.  
Traffic is heaviest on weekdays, indicating the need for optimized staff scheduling.  

## Data Structure
![Data Structure](/s1.png)  
The structure includes patient demographic tables, appointment records, referral data, satisfaction logs, and service feedback.  
Relationships were built in Power BI’s data model using patient IDs and appointment IDs as keys.  

## Data Model Overview
![Data Model](/m1.png)  
The model integrates multiple fact and dimension tables.  
- Fact tables: Patient visits, wait times, referrals  
- Dimension tables: Gender, race, appointment type, department, year  
Power BI relationships allowed accurate joins across dimensions and facts.  

## Analysis
- Adults account for most visits, followed by teenagers and middle childhood groups.  
- 4878 visits in 2020 compared to 4338 in 2019, showing year-on-year growth.  
- Weekday visits (6.6K) are significantly higher than weekend visits (2.6K).  
- Gender is balanced, with 51.1% male and 48.7% female.  
- Referral distribution is heavily skewed towards General Practice, followed by Orthopedics.  
- Race analysis shows diversity, with categories including African American, Asian, Native American, Pacific Islander, and White.  

## Dashboards
![Dashboard](/dash2.png)  
The dashboard consolidates all metrics into one interactive view.  
Filters enable drilldowns by time, referral type, age group, and race.  
Heatmaps highlight satisfaction across demographic groups.  

## Insights
- Adults represent the majority of ER visits.  
- Referrals are uneven, with most patients not being referred at all.  
- High wait times correspond to lower satisfaction.  
- Services are poorly rated or unrated, limiting patient feedback quality.  
- Workload peaks during weekdays, suggesting capacity challenges.  
- Race and age group interactions show unique wait time patterns, affecting satisfaction.  

## Recommendations
- Increase weekday staffing to handle high demand.  
- Reduce average wait times from 35 minutes to under 25 to improve satisfaction.  
- Introduce structured feedback collection to reduce the 75.1% unrated service issue.  
- Allocate more resources to General Practice and Orthopedics due to referral demand.  
- Focus patient education on adults, who dominate ER visits.  
- Monitor satisfaction heatmaps by demographic to target improvements.  
- Continue end-to-end use of Power BI for ongoing monitoring, reporting, and decision support.  

