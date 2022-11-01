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
The aim was to understand how profitable an investment in a particular channel will be over time and determine the benchmark/walk-away point for the investment. Historic data was analyzed and a model for the forecast was prepared.


## Technique
When looking at the LTV calculation used by the company I identified that the calculation didn’t take into account future purchases (only renewals of subscriptions already purchased). Therefore, I created SQL that pulls the historic data for purchases made by clients.

Then I created a simple model that estimates how many purchases there is going to be from specific registration cohort (and for specific acquisition channel) in different periods.

Based on this we were able to calculate LTV more accurately for each registration cohort taking into consideration future purchases as well. 
