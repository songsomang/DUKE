# Air Quality and Sickle Cell Disease: Exploratory Analysis

## Project purpose

This project processes course-provided air-quality measurements from 2018 through April 2020 into one record per date. It summarizes carbon monoxide (CO), fine particulate matter (PM2.5), and ozone (O3), and explores their monthly patterns.

The analysis is motivated by research on potential associations between air pollution and health-system utilization among people with sickle cell disease (SCD) in Durham County, North Carolina. This project provides exploratory summaries of air-quality data; it does not estimate an association between air pollution and SCD utilization.

The report includes annual minimum and maximum summaries for each pollutant, monthly CO and O3 averages with 95% confidence intervals, and monthly PM2.5 patterns by year.

## Data source

The course-provided CSV files contain measurements from the U.S. EPA air-quality monitor at Raleigh-Durham International Airport (RDU):

- `AQ_2018.csv`
- `AQ_2019.csv`
- `AQ_2020.csv`

The 2020 file covers January through April only. The original files are stored unchanged in `data/`.

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
        ├── Project2.Rmd
        ├── Project2.docx
        └── README.md
```

## How to reproduce

Open `DUKE.Rproj` in RStudio. Install the required packages if they are not already installed:

```r
install.packages(c("tidyverse", "here", "rmarkdown"))
```

To create or update the Word report, run:

```r
rmarkdown::render(
  input = here::here(
    "BIOSTAT-721",
    "Project2",
    "Project2.Rmd"
  ),
  output_format = "word_document"
)
```

The rendered report is saved as `Project2.docx` in the same folder as the R Markdown file.

## Author and date

Author: Somang Elena Song  
Date: November 20, 2026
