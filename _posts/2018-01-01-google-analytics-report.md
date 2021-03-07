---
layout: post
title:  "Data Studio Report for B2B customers "
info: E-branding report in Data Studio Report based on Google Analytics data for B2B customers
tech: Google Analytics, JavaScript, Google Sheets, Google Data Studio
dates: "2018/01" 
categories: Experteer
tags: Google-Analytics JavaScript Google-Sheets
---

## Goal
The goal was to create report for our B2B customers that shows exposure they get to their brand on our website. Requirement were for report to be refreshed automatically by account manager and to be able to use screenshot of visuals in presentation for the client.


## Techique
Main data source for this report is Google Analytics. Howeever some additional data was added manually by account managers. Therefore, it was decided to use Google Analytics API in Google Sheets to extract data for each client separately (based on a filter) and join it together with manual data. This also allowed for quick on demand refresh by account manager without introducing any additional tool into their aresenal.

As a first step I crated a schema with predefined primary key to combine both data sources. Then I created a filter for each client and defined these filters and clients in Google Sheets and Google Analytics API.

Once data was pulled from Google Analytics into the sheet I wrote Google App script (JavaScript) that cleans up and prepares the data to use in Google Data Studio for report preparation.

The last step was to join 2 data sources in Google Data Studio and visualize the data in the way that will allow to easily add it into the presentation.

 
