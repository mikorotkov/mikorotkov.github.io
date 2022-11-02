---
layout: post
title:  "Migration to Google Big Query"
info: "Migration of DWH from SQL Server to Google Big Query"
tech: Python, Apache Airflow, Google Cloud Platform, Git, Google Composer
dates: "2020/09 ~ 2021/09"
categories: Experteer
tags: Python Apache-Airflow BigQuery Google-Composer
---

## Goal
The goal was to gain speed and scalability in data processing by migrating to a Google Cloud solution. This requires
design of the table relationships, optimization of SQL queries, and implementation of ETL data pipelines with
Apache Airflow.  


## Technique
I'm leading the process of migrating on-premise infrastructure (SSIS and Microsoft SQL Server) to the Google Cloud platform. 
Data pipelines consisted of
Fivetran as a data ingestion tool
Apache Airflow as an orchestration tool
Transformations and loading of data were done with vanilla SQL
Google BigQuery as a data warehouse
