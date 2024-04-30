# Data Analysis Summary: Heineken Brand Awareness and Sales Impact

**Author:** Meitong Chen  
**Date:** February 28, 2024  
**Output:** HTML Document  

## Overview
This document details a statistical analysis performed on Heineken's brand awareness and sales data. The analysis examines the impact of advertising, environmental factors, and external events on sales volumes and brand awareness.

## Libraries Used
- `readxl`: For reading Excel files.
- `dplyr`: For data manipulation.
- `Hmisc`: For advanced statistical functions.
- `MASS`: For statistical methods.

## Data Preparation
Data was sourced from a file named `Heineken.xlsx`. Initial exploration involved viewing the first few records to understand the dataset's structure.

## Feature Engineering
New variables were created to capture lag effects in sales and awareness, which are crucial for time series analysis. The dataset was also refined by selecting relevant columns and renaming them for clarity.

## Statistical Modeling
Three linear models were constructed:
1. **Model 1 (`m1`)**: Explores the effect of lagged brand awareness and out-of-home advertising on current awareness.
2. **Model 2 (`m2`)**: Similar to `m1` but includes social media advertising as a predictor.
3. **Model 3 (`m3`)**: A comprehensive model predicting sales based on lagged sales, current awareness, advertising expenditures, average temperature, and COVID-19 stringency index.

## Key Findings
- Lagged awareness significantly influences current awareness.
- Both social media advertising and out-of-home advertising significantly affect brand awareness.
- Sales are influenced by a combination of lagged sales, current awareness, advertising types, temperature, and COVID-19 restrictions.

## Mediation Analysis
Mediation effects were calculated to understand the indirect effects of advertising through brand awareness on sales. Total effects, including direct and mediated pathways, were also quantified.

## Monte Carlo Simulations
To account for the variability in estimates and to assess the robustness of our results, Monte Carlo simulations were performed:
- Generated distribution of estimates based on the variability observed in the original data.
- Calculated potential outcomes over 1000 simulations to provide a range of possible effects.

## Conclusions
The analysis provides valuable insights into the factors driving Heineken's brand awareness and sales, highlighting the importance of both traditional and digital advertising. The findings also underscore the impact of external factors like weather conditions and public health measures.


