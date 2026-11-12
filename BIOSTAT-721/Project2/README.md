# Air Quality and Sickle Cell Disease: Exploratory Analysis

## Project purpose

This project processes raw air-quality monitor measurements from 2018–2020 into one record per day and explores monthly patterns in carbon monoxide (CO), fine particulate matter (PM2.5), and ozone (O3). The analysis is motivated by research on potential associations between air pollution and health-system utilization among people with sickle cell disease (SCD) in Durham County, North Carolina. This project provides exploratory summaries of air-quality data; it does not estimate the association between pollution and SCD utilization.

The analysis will create annual minimum and maximum summaries for each pollutant, examine monthly CO and O3 averages with 95% confidence intervals, and display monthly PM2.5 patterns by year.

## Data source

The course-provided CSV files contain raw measurements from the U.S. EPA air-quality monitor at Raleigh-Durham International Airport (RDU):

- `AQ_2018.csv`
- `AQ_2019.csv`
- `AQ_2020.csv`

The 2020 file covers January through April only.

## Repository structure

This project is located at `BIOSTAT-721/Project2/` in the `DUKE` repository.

```text
DUKE/
└── BIOSTAT-721/
    ├── Project1/
    └── Project2/
        ├── data/
        │   ├── AQ_2018.csv
        │   ├── AQ_2019.csv
        │   └── AQ_2020.csv
        ├── R/
        │   └── process_air_quality.R
        ├── report/
        │   ├── air_quality_report.Rmd
        │   └── air_quality_report.docx
        ├── BIOSTAT-721-Project-2.Rproj
        └── README.md

## Author and date
Author: Elena Song
Date: November 11, 2026
