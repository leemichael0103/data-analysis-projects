# Central Valley Air Quality Analysis (2023)

A Python-based analysis of PM2.5 and ozone air quality across California's Central Valley, using EPA Air Quality System (AQS) public data.

## Motivation

The Sacramento Valley and San Joaquin Valley consistently rank among the worst air quality regions in the United States. This analysis examines 2023 monitoring data to understand which counties have the most severe pollution, which months are worst, and how conditions compare across the two air basins. This work directly relates to California's State Implementation Plan (SIP) development process under the Clean Air Act.

## Key Questions

1. Which Central Valley counties have the highest mean annual PM2.5?  
2. How many days did each county exceed the EPA 24-hour PM2.5 standard (35 ug/m3)?  
3. Which months are worst for PM2.5 and ozone?  
4. How do the Sacramento Valley and San Joaquin Valley compare?

## Data Source

EPA Air Quality System (AQS) Daily Summary Data — freely available at: [https://aqs.epa.gov/aqsweb/airdata/download\_files.html](https://aqs.epa.gov/aqsweb/airdata/download_files.html)

Files used:

- `daily_88101_2023.csv` — PM2.5 daily measurements (Parameter 88101\)  
- `daily_44201_2023.csv` — Ozone daily measurements (Parameter 44201\)

## How to Run

pip install pandas numpy matplotlib

\# Download data files from EPA AQS link above

\# Place CSV files in the same directory as the script

python air\_quality\_analysis.py

## Key Findings

- Winter months (December through February) produce the highest PM2.5 concentrations due to temperature inversions trapping pollutants near the surface  
- Summer months (June through September) produce the highest ozone concentrations due to photochemical reactions in high temperatures and sunlight  
- The San Joaquin Valley consistently records worse PM2.5 levels than the Sacramento Valley  
- Fresno, Kern, and Tulare counties record the most days exceeding the EPA 24-hour PM2.5 standard

## Tools Used

- Python 3.x  
- Pandas — data loading, cleaning, and analysis  
- NumPy — statistical calculations  
- Matplotlib — data visualization

## About

This project was developed as part of a portfolio demonstrating applied data analysis skills in environmental and air quality contexts. The analysis techniques used here — data cleaning, trend analysis, AQI categorization, and visualization — are directly applicable to emissions inventory development and air quality planning work.

Author: Michael Lee B.S. Physics, University of California Davis, 2025  
