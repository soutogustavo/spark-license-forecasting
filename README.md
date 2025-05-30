# Forecasting Liquor License Issuance in Chicago (Spark + Databricks)

This project explores whether it's possible to forecast the number of liquor (new) licenses issued monthly in Chicago using open city data and PySpark on Databricks.

## Goals

- Analyze historical trends
- Engineer time-based features (lags, rolling stats, cyclic month encodings)
- Train scalable ML models in Spark (Linear Regression, Random Forest, GBT)
- Evaluate the predictive power of internal patterns
- Understand the limits of forecasting administrative processes

## Dataset

- Source: [Chicago Data Portal – Liquor Retail Licenses](https://data.cityofchicago.org)
- Time range: 2000–2025
- Frequency: Monthly aggregation of new licenses issued

## Tools & Stack

- Apache Spark (PySpark)
- Databricks (Community Edition)
- MLlib (for regression models)
- Delta Lake (data storage and versioning)

## Results

Despite careful feature engineering and model testing, all models (including GBT and RF) underperformed compared to a simple baseline. This suggests that license issuance is not easily predictable from past values alone and is likely influenced by external, non-observed factors (e.g., policy changes, local events).

## Key Takeaway

Not all patterns can be learned from internal historical data. Understanding when machine learning is appropriate is a valuable insight in itself.

## Notebooks & Artifacts

You can explore the full analysis and model pipeline in the [Databricks notebook](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1577492776175845/1846952264539377/4308252803629806/latest.html).

---

