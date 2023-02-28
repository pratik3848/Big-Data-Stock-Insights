# BIG DATA STOCK INSIGHTS

## Overview

This project is an implementation of big data stock insights using Spark, Dataproc, GCS, and BigQuery. The goal of this project is to analyze daily and historical stock data of 1500+ stocks to provide valuable insights and improve decision making.

## Data Source

The data source used in this project is the Polygon.io API, which provides real-time and historical stock data, as well as news data for all stocks. The project also includes historical data of the last 40 years of all stocks' high, low, and end-of-day (EOD) price.

## Data Pipeline

The data pipeline includes the following steps:

1.  Data collection using Spark on Dataproc from the Polygon.io API.
2.  Data optimization using Spark and partitioning it by year, month, and day.
3.  Storing the optimized data in GCS.
4.  Loading the optimized data from GCS to the data warehouse using Spark on Dataproc and BigQuery.
5.  Connecting the data warehouse to PowerBI to create multiple visualizations to get stocks news and history as well as new data.

## Conclusion

This project showcases the implementation of a scalable big data pipeline for daily and historical stock analysis, improving query response time and providing valuable insights to make better decisions. The automation of the pipeline using Airflow reduces manual effort and ensures the latest insights and news are always available on the dashboard.
