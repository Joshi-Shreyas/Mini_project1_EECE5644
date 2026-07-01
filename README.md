# Mini Project: Retail Data Cleaning

## Overview

This project cleans and analyzes the UK Online Retail dataset. The goal is to create a reliable completed-sales dataset and answer business questions about revenue, products, countries, customers, and data quality.

## Dataset

Dataset: E-Commerce Data  
Source: https://www.kaggle.com/datasets/carrie1/ecommerce-data

Place `data.csv` in the project folder before running the notebook.

The dataset should be loaded with:

```python
pd.read_csv("data.csv", encoding="ISO-8859-1")
```

## Files

```text
Mini_Project_Assignment_P1.ipynb
data.csv
clean_online_retail.csv
data_dictionary.md
findings_summary.md
cleaning_decisions_log.md
README.md
requirements.txt
```

## How to Run

Install the required packages:

```bash
pip install -r requirements.txt
```

Open and run the notebook:

```bash
jupyter notebook Mini_Project_Assignment_P1.ipynb
```

Run all cells from top to bottom. The notebook will generate:

```text
clean_online_retail.csv
```

## Cleaning Summary

The notebook completes the required pandas cleaning techniques, including loading, profiling, filtering, replacing values, renaming columns, handling missing values, removing invalid rows, dropping duplicates, grouping, aggregating, resampling, concatenating, and merging.

The final cleaned dataset removes cancellations, returns, bad prices, invalid quantities, duplicates, and non-product rows.

## Output

The cleaned dataset is saved as:

```text
clean_online_retail.csv
```

The final business answers are summarized in:

```text
findings_summary.md
```
