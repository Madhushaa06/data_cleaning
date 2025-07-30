
# Data Cleaning Report: Hotel Booking Demand Dataset

## Executive Summary
This report documents the cleaning process for the Hotel Booking dataset with over 119,000 records. The goal was to prepare the data for analysis by resolving missing values, duplicates, and inconsistencies.

## Data Quality Assessment
- Original Rows: 119,390
- Issues Found:
  - Missing values in 'children', 'country', 'agent', 'company'
  - ~30 duplicate rows
  - Outliers in 'lead_time', 'adr'
  - Some bookings with 0 guests

## Cleaning Methodology
- Replaced NaN with 0 or mode for key columns
- Removed duplicates
- Handled outliers using IQR
- Fixed 0-guest bookings and standardized text fields

## Results and Impact
- Final Row Count: 51220  
- All missing values handled  
- Dataset is now analysis-ready  

## Recommendations
- Enforce input validation during data collection
- Use NULL flags instead of leaving blanks
