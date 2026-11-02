Phase A – Exploratory Data Analysis (EDA) Figures

This directory contains the visual outputs generated during Phase A of the P02: Next-Day Air Quality Prediction for an Indian City project.

The visualizations are based on historical air-quality observations from Delhi, extracted from the original Air Quality Data in India dataset.

These figures help understand the dataset's quality, identify missing-data patterns, examine historical PM2.5 variations and investigate seasonal pollution behaviour before developing predictive models.

1. Missingness Heatmap

File: missingness_heatmap.png

Description

This heatmap visualizes the distribution of missing values across different air-quality parameters over the observation period.

Objectives
Identify pollutants and attributes with substantial missing data.
Observe periods with frequent missing observations.
Understand the extent of data incompleteness.
Support decisions regarding feature selection and missing-value handling.
Relevance

Missing data can affect model training, feature engineering and prediction reliability. This visualization supports the development of a documented missing-data policy for subsequent preprocessing stages.

2. PM2.5 Over Time

File: pm25_over_time.png

Description

This time-series plot illustrates daily PM2.5 concentration variations in Delhi across the available observation period.

Objectives
Examine historical PM2.5 fluctuations.
Identify possible seasonal and temporal pollution patterns.
Investigate periods of unusually high or low PM2.5 concentrations.
Observe pollution-level changes around the 2020 COVID-19 lockdown period.
Relevance

Understanding historical pollution behaviour helps identify temporal dependencies and potential patterns useful for next-day PM2.5 forecasting.

3. Monthly PM2.5 Distribution

File: pm25_monthly_distribution.png

Description

This visualization compares the distribution of PM2.5 concentrations across different calendar months.

Objectives
Examine monthly differences in pollution levels.
Identify potential seasonal variations.
Compare the spread and variability of PM2.5 measurements.
Identify unusually high observations and potential outliers.
Relevance

Air pollution can exhibit seasonal behaviour due to changes in weather, atmospheric conditions and human activities. Understanding monthly distributions helps determine whether calendar-based features may contribute to predictive performance.

4. Summary of Visualizations
Visualization	Primary Purpose	Project Relevance
Missingness Heatmap	Identify missing-data patterns	Missing-data policy
PM2.5 Over Time	Examine historical pollution trends	Time-series forecasting
Monthly PM2.5 Distribution	Investigate seasonal variation	Calendar feature engineering
5. Project Information
Project: P02 – Next-Day Air Quality Prediction
Phase: Phase A – Problem Understanding and Exploratory Data Analysis
Selected City: Delhi, India
Dataset: city_day.csv
Primary Regression Target: Next-day PM2.5 concentration
Classification Target: Next-day AQI_Bucket
6. Important Notes
All visualizations are generated through the Phase A EDA notebook.
Missing observations are not automatically treated as zero.
The visualizations represent exploratory findings and do not establish causal relationships.
Observations and patterns identified here guide subsequent preprocessing and modelling decisions.

These figures establish the exploratory foundation for the project's next stages: baseline development, feature engineering, predictive modelling and evaluation.
