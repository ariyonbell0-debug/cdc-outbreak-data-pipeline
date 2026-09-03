# Public Health Trend Analysis Pipeline

An automated data engineering pipeline built with Python and Pandas to ingest clinical outbreak records, standardize epidemiological MMWR weeks, compute disease incidence rates per 100,000 residents, and generate automated surveillance trends.

##  Overview

This project provides a robust, object-oriented workflow for public health data analytics. It bridges clinical operations and epidemiological reporting by automating data cleaning, calculating standardized disease incidence metrics, and smoothing trends via rolling averages for public health surveillance.

##  Tech Stack

- **Python** (Pandas, NumPy, Matplotlib)
- **Data Engineering:** Automated synthetic data generation fallback, missing data integrity handling, and timestamp standardization
- **Epidemiological Metrics:** MMWR/ISO week extraction and standardized incidence calculations per 100,000 residents

##  Key Features

- **Data Ingestion & Cleaning:** Safely ingests raw clinical surveillance logs or generates robust synthetic outbreak datasets.
- **MMWR Week Standardization:** Converts raw timestamps into standardized epidemiological year and week numbers for temporal tracking.
- **Incidence Normalization:** Computes population-adjusted disease rates (`Incidence_Per_100k`) to ensure accurate cross-facility comparisons.
- **Trend Smoothing:** Calculates rolling averages to filter out short-term noise and highlight true epidemiological outbreaks.

##  Usage

To run the pipeline and output processed surveillance summaries, execute:

```bash
python pipeline.py
