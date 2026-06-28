# Central Valley Air Quality Analysis (2023)

A Python-based analysis of air quality across California's Central Valley, using EPA Air Quality System (AQS) public data.

## Motivation

The Sacramento Valley and San Joaquin Valley consistently rank among the worst air quality regions in the United States. I live in Woodland, CA in the Sacramento Valley — one of the areas directly responsible for some of California's most persistent air quality challenges. This analysis examines 2023 EPA monitoring data to understand which counties have the most severe pollution, how conditions compare across the two air basins, and what the data reveals about the scale of the nonattainment problem in the Central Valley. This work is directly relevant to California's State Implementation Plan (SIP) development process under the Clean Air Act, which drives emission reduction requirements for PM2.5 and ozone in these regions.

## Key Questions

1. Which Central Valley counties have the most unhealthy air days?
2. How do the Sacramento Valley and San Joaquin Valley compare across AQI categories?
3. Which counties recorded the highest maximum AQI values in 2023?
4. How does the AQI category breakdown differ between the two air basins?

## Key Findings

- Tulare County had 82 unhealthy air days in 2023, the worst in the Central Valley
- The San Joaquin Valley averaged 37.5 unhealthy days per county versus only 3.8 for the Sacramento Valley
- Kern County recorded the highest sustained AQI levels of any Central Valley county with 70 unhealthy days
- The San Joaquin Valley consistently shows worse air quality across every AQI category compared to the Sacramento Valley
- Fresno and Tulare counties exceed EPA thresholds at rates that reflect longstanding nonattainment designations under the Clean Air Act

## Data Source

EPA Air Quality System (AQS) AQI by County Annual Summary Data, freely available at:
https://aqs.epa.gov/aqsweb/airdata/download_files.html

File used: annual_aqi_by_county_2023.csv (from the AQI by County tab, 2023)

## How to Run

Open Air_Quality_Analysis.ipynb in Google Colab or Jupyter Notebook. When prompted, upload the annual_aqi_by_county_2023.csv file and run all cells. The notebook will print a county summary table, key findings, and generate a four-panel visualization saved as central_valley_air_quality_2023.png.

## Tools Used

- Python 3
- Pandas for data loading, filtering, and analysis
- NumPy for statistical calculations
- Matplotlib for data visualization

## About

This project was developed as part of a data analytics portfolio demonstrating applied Python and environmental data analysis skills. The analytical techniques used here including data cleaning, AQI categorization, air basin comparison, and visualization are directly applicable to emissions inventory development, air quality planning, and State Implementation Plan work.

## Author

Michael Lee
B.S. Physics, University of California Davis, 2025
github.com/leemichael0103
