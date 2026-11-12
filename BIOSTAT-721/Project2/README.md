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
├── DUKE.Rproj
└── BIOSTAT-721/
    ├── Project1/
    └── Project2/
        ├── data/
        │   ├── AQ_2018.csv
        │   ├── AQ_2019.csv
        │   └── AQ_2020.csv
        ├── process_air_quality.R
        ├── air_quality_report.Rmd
        ├── air_quality_report.docx
        └── README.md
```

## How to reproduce

1. Open `DUKE.Rproj` at the repository root in RStudio.
2. Install the packages used by the analysis: `tidyverse`, `here`, `rmarkdown`, and `lintr`.
3. Render `BIOSTAT-721/Project2/report/air_quality_report.Rmd` to Microsoft Word. The report will use the function in `BIOSTAT-721/Project2/R/process_air_quality.R` and the CSV files in `BIOSTAT-721/Project2/data/`.

`lintr` is used for code-style checks and is not required to render the report.

## Author and date
Author: Elena Song
Date: November 11, 2026
