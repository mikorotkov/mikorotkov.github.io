---
layout: post
title:  "Implementation of reporting hub with Tableau"
info: "Implementation of reporting hub with Tableau"
tech: Tableau, dbt, Git
dates: "2022/01 ~ 2022/05"
categories: Ryte
tags: dbt Tableau git
---

## Goal
The goal is to have a central reporting hub for reports in the company  


## Technique
After analyzing the reporting landscape of the company, it became clear that it was difficult for people to discover the data they needed to make a decision. Reports were created in various systems (Google Data Studio, Google Sheets, etc.) and were shared among people unsystematically.
This hindered the operations of the company because people preferred making gut-feeling decisions and struggled to get the reliable data they needed.

Instead of having reports decentralized, across various systems, we decided to create a reporting hub that all the people in the company would have access. Tableau was chosen after a thorough evaluation of multiple other visualization and reporting solutions.

In addition, we created a metrics catalog and business glossary to have clear definitions of KPIs and metrics across an organisation. 
Finally, a simple yet efficient strategy was created to manage access to sensitive data within the organisation.