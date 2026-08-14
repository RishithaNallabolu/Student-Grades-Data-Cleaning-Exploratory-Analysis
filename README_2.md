# Student Grades — Data Cleaning & Exploratory Analysis

A data cleaning and exploratory analysis project on a student academic records dataset, built with Python and Pandas. The focus is on taking a raw dataset from first look through to a verified, analysis-ready state — a foundational step in any data project.

## Dataset

`grades.csv` — 100 student records with the following fields:

| Column | Description |
|--------|-------------|
| ID | Unique student identifier |
| Name | Student name |
| GPA | Grade point average (scale: 0–4.0) |
| Major | Declared academic major (13 unique majors represented) |

## Project workflow

**1. Data loading and first inspection**
Loaded the CSV into a Pandas DataFrame and examined its structure — checking the top and bottom rows to understand the shape and content of the data before doing anything else.

**2. Descriptive statistics**
Generated summary statistics (mean, standard deviation, quartiles, min/max) across the numeric fields to understand the overall distribution of student GPAs — for example, the dataset spans a GPA range of 1.03 to 3.97, with a mean around 2.48.

**3. Duplicate detection and removal**
Programmatically scanned the full dataset for exact duplicate rows and removed any found, then re-verified the dataset to confirm none remained — an essential check before drawing any conclusions from the data.

**4. Missing value handling**
Checked every row and column for missing (null) values, removed incomplete records, and verified the cleaned dataset was fully populated with no gaps.

**5. Verification**
Re-ran checks after each cleaning step to confirm the transformations worked as intended, rather than assuming success.

## Why this matters

Real-world datasets are rarely clean. Before any statistical analysis, visualization, or modeling can be trusted, the underlying data has to be verified — free of duplicates, gaps, and inconsistencies. This project demonstrates that foundational data-cleaning workflow using core Pandas operations.

## Tools

Python, Pandas

## Key result

A fully cleaned, duplicate-free, and null-free dataset of 100 student records, verified and ready for further analysis (e.g., GPA trends by major, correlation studies, or predictive modeling).
