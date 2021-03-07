---
layout: post
title:  "Expected Profitability Forecast"
info: "Expected Profitability Forecast for LTV calculation"
tech: SQL, SSIS, Excel
dates: "2018/05 ~ 2018/07" 
categories: Experteer
tags: SQL SSIS Excel
---

## Goal
The aim was to understand how profitable an investment in particular channel will be over time and determine
the benchmark/walk-away point for the investment. Historic data was analyzed and model for the forecast was
prepared. 


## Techique
When looking at LTV calculation used by the company I identified that calculation didn't take into account future purchases (only renewals of subscriptuions already purchased). Therefore, I created SQL that pulls the historic data for purchases made by clients. 

Then I created a simple model that estimates how many purchases there is going to be from specific registration cohort (and for specific acquisition channel) in different time periods. 

Based on this we were able to calculate LTV more accurately for each registration cohort taking into consideration future purchases as well. 
