# BIOSTAT 721 — Project 1
## Clinical Data Cleaning and Descriptive Summaries

This project uses R and R Markdown to prepare and summarize patient-level and encounter-level data. It focuses on data cleaning, combining datasets, and presenting descriptive results in a reproducible report.

## Project Overview

The source data contain demographic and clinical information for 50 patients and records from 550 patient encounters. The datasets were linked using the medical record number (MRN), producing an encounter-level analytic dataset with 550 rows and 14 variables.

The project distinguishes between patient-level summaries and encounter-level summaries so that patients with multiple visits are not counted repeatedly when describing patient characteristics.

## Data Preparation

- Inspected variable types, missing values, and potentially invalid observations.
- Converted dates of birth and encounter dates to date variables.
- Recoded six negative BMI values as missing.
- Set 14 WBC measurements below the detection limit to 1, following the project instructions.
- Combined patient characteristics with encounter records using MRN.

## Descriptive Summaries

- Categorized white blood cell (WBC) measurements as Low, Normal, High, or Not Taken.
- Created an encounter-level table showing counts and percentages for each WBC category.
- Created a patient-level Table 1 summarizing race, ethnicity, financial class, hypertension, congestive heart failure, and diabetes.

## View the Report

[Open the formatted HTML report](https://songsomang.github.io/DUKE/DUKE%20721/Project/Song_Elena_Project1.html)

## Files

- `Song_Elena_Project1.Rmd`: R Markdown source document.
- `Song_Elena_Project1.html`: Rendered report with data preparation output and summary tables.
- `Data/`: Input data used in the project.

## Tools

R, R Markdown, tidyverse, here, lubridate, gt, and gtsummary.
