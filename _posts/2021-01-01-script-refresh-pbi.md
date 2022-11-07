---
layout: post
title:  "Script to refresh Power BI report programmatically"
info: "Script to refresh Power BI report programmatically"
tech: Python, Apache Airflow, Google Cloud Platform, Power BI, Google Composer
dates: "2021/01 ~ 2021/01"
categories: Experteer
tags: Python Apache-Airflow BigQuery Google-Composer Power-BI
---

## Goal
We wanted to have an operator in Airflow to trigger a refresh of Power BI reports after the data refresh has finished. This allowed the flexibility to split and combine dags and trigger reports refresh at various steps of the dag.


## Technique
The function receives a dictionary that should contain arguments `pbi_app` (app name exactly as in PBI) and `name` (report name exactly as in PBI).

It reads credentials (email and password) from environmental variables `PBI_USER`, `PBI_PASSWORD`, and `CLIENT_ID` that need to be defined in a local or Google Composer environment (if used as an Airflow task in Google Composer). 

It then makes a call to PBI API to first retrieve group_id based on the app name (function get_group_id) and then retrieves dataset_id to be refreshed based on the report name and group_id retrieved earlier (function get_dataset_id).

Finally, it refreshes the dataset in PBI.

The [script](https://github.com/mikorotkov/refresh-pbi-report).
