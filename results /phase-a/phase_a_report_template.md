
# P02: Next-Day Air Quality for an Indian City

## 1. Objective
The project investigates whether historical pollutant readings
and calendar information can predict next-day PM2.5 concentration
and next-day AQI category.

## 2. City selection
Selected city: Delhi

Justification:
The project brief identifies Delhi as a useful starting city
because of its broad pollution range and comparatively complete
record. This choice must be checked against the observed
missingness and date coverage.

## 3. Dataset
Source:
https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india

File: city_day.csv

The dataset contains city-level daily pollution measurements
and AQI information.

## 4. Data quality
Describe:
- Date coverage
- Missing calendar dates
- Duplicate city-date records
- Missingness by column and year
- Features with extensive or long-duration gaps

See results/missingness_by_year.csv.

## 5. Missing-data policy
Explain the decisions in results/missing_data_policy.md.
Revise the provisional policy after reviewing the actual
missingness statistics.

## 6. PM2.5 trends
Discuss the observed time-series plot and monthly distribution.
Investigate winter spikes and the 2020 lockdown period.
Do not claim a pattern that is not visible in the data.

## 7. Limitations
Discuss missing measurements, monitoring coverage, possible
sensor issues and the limitations of a single-city dataset.

## 8. Next steps
Build the persistence baseline and first time-ordered linear
regression model in Phase B.
