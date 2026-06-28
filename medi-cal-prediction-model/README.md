# California Hospital Medi-Cal Rate Prediction Model

A machine learning classification model that predicts whether a California 
county has high Medi-Cal utilization based on demographic and healthcare 
utilization features.

## Problem Statement

California counties vary significantly in their Medi-Cal utilization rates,
from 15% in wealthy suburban counties to over 40% in rural Central Valley
counties. Understanding which county characteristics drive high Medi-Cal
rates helps healthcare planners allocate resources and design targeted
programs for underserved populations.

## Approach

Binary classification using a Random Forest model. The target variable is
whether a county's Medi-Cal rate exceeds the statewide median of 28%.

## Data Sources

1. HCAI Hospital Inpatient Characteristics by Patient County of Residence
   https://data.chhs.ca.gov/dataset/hospital-inpatient-characteristics-by-patient-county-of-residence

2. CHSP County Health Status Profiles 2024
   https://data.chhs.ca.gov/dataset/county-health-status-profiles

## Features Used

- Child poverty rate (% of children under 18 in poverty)
- Self-pay rate (% of hospital discharges paid out of pocket)
- Medicare rate (% of hospital discharges covered by Medicare)
- Private coverage rate (% of hospital discharges with private insurance)
- Other government coverage rate
- Total hospital discharges (county volume)

## Results

- Cross-validation accuracy: 91%
- Test set accuracy: 83%
- Overall accuracy on full dataset: 96%
- 55 of 57 counties correctly classified

## Key Findings

- Child poverty rate is the strongest predictor of high Medi-Cal utilization
- Counties with child poverty rates above 20% are almost always high Medi-Cal
- The two misclassified counties (Sacramento and Shasta) both fall within 2
  percentage points of the statewide median, where boundary cases are expected
- Central Valley counties (Merced, Kern, Tulare, Fresno) are correctly
  identified as high Medi-Cal in every model run

## Tools Used

- Python, SQL (pandasql), Pandas
- Scikit-learn (RandomForestClassifier, train_test_split, cross_val_score)
- Matplotlib

## Author

Michael Lee
B.S. Physics, UC Davis 2025
github.com/leemichael0103
