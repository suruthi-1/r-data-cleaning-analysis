# Data Cleaning and Preliminary Analysis in R

Internship task: data cleaning, preprocessing and exploratory analysis of the
msleep (mammal sleep) dataset using R.

## Files
- `data_cleaning_analysis.docx` - final report with code, outputs and plots
- `data_cleaning_analysis.Rmd` - R Markdown source (code + explanations)
- `msleep_clean.csv` - cleaned dataset

## What was done
- Missing values: dropped columns with >50% missing, "unknown" for categories, group-median imputation
- Outliers: IQR rule, kept and handled with log transformation
- Normalisation: z-score and min-max scaling
- Encoding: one-hot, ordinal and frequency encoding
- EDA: summary statistics, visualisations and correlation analysis

## How to run
    install.packages(c("tidyverse", "knitr", "rmarkdown"))
    rmarkdown::render("data_cleaning_analysis.Rmd")
