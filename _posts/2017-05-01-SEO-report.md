---
layout: post
title:  "SEO Report based on Search Console API data"
info: SEO Report based on data exported from Search Console API
tech: Google Search Console, SQL, SSIS, Excel, PowerQuery
dates: "2017/05 ~ 2017/07" 
categories: Experteer
tags: SQL SSIS Excel Power-BI
---

## Goal
The goal was to add Search Console data to SEO reporting, since data there is stored only for last 3 months. API 
was implemented and ETL process designed in SSIS to save the data in DWH. The data was then added into the 
SEO report.


## Techique
1. In coordination with tech team script was created to extract data from Google Search Console and save it as csv on shared drive
2. The package that I created in SSIS, uploaded the data to staging table in Microsoft SQL Server. Data was then updated in fact table, with integrated check to make sure no duplicates are created.
3. This data was then pulled into the report file with, transformed and joined with other data sources (such as internal site data) in order to present SEO performance on a daily basis.




