# NYPD Shooting Incident Data Report

This repository contains a reproducible data science report analyzing the NYPD Shooting Incident Data. The project looks at reported shooting incidents in New York City and focuses on patterns by borough, year, time of day, and murder classification.

## Project Overview

The report uses R Markdown to import, clean, summarize, visualize, and model the NYPD shooting incident dataset. The main goal is to identify clear patterns in the data while also recognizing the limits of the analysis.

## Main Questions

- Which boroughs had the highest number of reported shooting incidents?
- How did reported shootings change over time?
- What time of day had the highest number of reported incidents?
- Do hour and borough help explain whether an incident was classified as a murder?

## Methods Used

- Data cleaning and transformation in R
- Missing value review
- Summary tables
- Data visualization with ggplot2
- Logistic regression model

## Key Findings

Brooklyn and the Bronx had the highest raw counts of reported shooting incidents, while Staten Island had the lowest count. Reported shootings declined through much of the 2010s, then increased sharply around 2020 and 2021. The time-of-day graph showed that reported shootings were more common later in the day and at night.

The logistic regression model used hour and borough to predict whether an incident was classified as a murder. The model was useful as a basic check, but hour and borough alone did not explain much of the difference between fatal and nonfatal shooting incidents.

## Limitations

This analysis uses raw counts, so the borough comparisons do not adjust for population size. The dataset also has missing values, especially for location details and perpetrator information. Because of this, the report should be treated as a descriptive analysis, not a full explanation of why shootings happen.

## Files

- `NYPD-Shooting-Incident-Data-Report.Rmd`: R Markdown source file
- `NYPD-Shooting-Incident-Data-Report.html`: Knitted HTML report
