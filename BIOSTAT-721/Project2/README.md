# Air Quality and Sickle Cell Disease: Exploratory Analysis

## Project purpose

This project summarizes course-provided air-quality measurements from the U.S. EPA monitor at RDU Airport from 2018 through April 2020. It reports annual minimum and maximum daily concentrations of CO, PM2.5, and O3; pooled monthly CO and O3 means with 95% confidence intervals; and monthly PM2.5 means by year. Motivated by research on air pollution and SCD-related health-system utilization in Durham County, this project analyzes air-quality data only and does not estimate an association with SCD utilization.

## Data source

The course-provided CSV files contain measurements from the U.S. EPA air-quality monitor at Raleigh-Durham International Airport (RDU). They cover 2018 through April 2020; the 2020 file includes January through April only. The original files are preserved unchanged in `data/`.

## File structure

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

- `data/` contains the original annual air-quality CSV files.
- `Project2.Rmd` contains the data-processing function and analysis.
- `Project2.docx` is the rendered Word report.
- `README.md` describes the project and how to reproduce the report.


## How to reproduce

1. Clone or download the `DUKE` repository, preserving its folder structure.
2. Open `DUKE.Rproj` at the repository root in RStudio.
3. If the required packages are not already installed, run:

   ```r
   install.packages(c("tidyverse", "here", "rmarkdown"))
   ```

4. To create or update the Word report, run this code in the R console:

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

You can also knit the report in RStudio by opening `BIOSTAT-721/Project2/Project2.Rmd` and selecting **Knit → Knit to Word**. The Word report is saved as `BIOSTAT-721/Project2/Project2.docx`.

## Author and date

- Author: Somang Elena Song
- Date: November 21, 2026