
# P02 Air Quality: Missing-Data Policy

## Selected city
Delhi

## Phase A findings
The dataset was reindexed to a continuous daily calendar.
The missingness tables distinguish the complete calendar from
the original observed records.

See:
- results/missingness_by_year.csv
- results/missingness_observed_rows.csv
- results/figures/missingness_heatmap.png

## Provisional policy for later modelling

1. Target values:
   - Do not impute missing PM2.5 target values.
   - Do not impute missing AQI_Bucket target labels.
   - Exclude samples whose required target is unknown.

2. Predictor columns:
   - Investigate the missingness of each predictor using the
     per-year tables and the training period.
   - Consider excluding a predictor if more than 40% of its
     values are missing in the training period, or if an
     entire year has no usable measurements.
   - Justify each exclusion using actual missingness results.

3. Remaining predictor values:
   - Start with median imputation for numeric predictors.
   - Fit imputers on training data only, preferably inside a
     scikit-learn pipeline.
   - Do not fit preprocessing on the complete dataset.

4. Calendar gaps:
   - Retain a continuous daily index.
   - Do not treat a previous available row as yesterday unless
     it is actually the previous calendar day.
   - Do not forward-fill long gaps automatically.

5. Evaluation:
   - Use time-ordered splits.
   - Apply the same test dates when comparing models and the
     persistence baseline.
   - Report the amount of data excluded by preprocessing.

## Finalisation
Review the missingness tables before confirming which
predictors to retain or drop. Update this policy with the
actual column names and observed percentages.
