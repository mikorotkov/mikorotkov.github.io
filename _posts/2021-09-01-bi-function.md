---
layout: post
title:  "Creation of Business Intelligence Function in the Company"
info: "Creation of Business Intelligence Function in the Company"
tech: Snowflake, dbt, Tableau, Git
dates: "2021/09 ~ 2022/02"
categories: Ryte
tags: Snowflake dbt tableau git
---

## Goal
Goal is to create business intelligence department in the company.  


## Techique
By analysing the data needs and data literacy of the stakeholders, I was able to define the startegy and the roadmap for its implemetation. 
The work started with assesing and comparing multiple tools that can be used for different parts of BI infrastructure. At the same time we started looking at the data sources and developing a strategy for storing the data in the efficient yet easily usable way.

Snowflake was chosen as a cloud dwh plaform, because of it's ability to control usage and cost on agranular level and ability to control access on a granular level.

dbt was chosen as a data transformation tool for the dwh, because of it flexibility, ability to generate documentation and it's approach to SQL as code.

DWH itself was designed in 3 layers to better control access to sensitive data such as PII. 

Below is schematic design of DWH developed:
<img class="dropshadowimg" src="/assets/img/2021-09-01-dwh-design.jpg" alt="DWH design schema" />