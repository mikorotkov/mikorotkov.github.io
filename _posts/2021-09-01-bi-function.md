---
layout: post
title:  "Creation of Business Intelligence Function in the Company"
info: "Creation of Business Intelligence Function in the Company"
tech: Snowflake, dbt, Tableau, Git
dates: "2021/09 ~ 2022/02"
categories: Ryte
tags: Snowflake dbt Tableau git
---

## Goal
Goal is to create business intelligence department in the company.  


## Technique
By analysing the data needs and data literacy of the stakeholders, I was able to define the startegy and the roadmap for its implemetation. 
The work started with assesing and comparing multiple tools that can be used for different parts of BI infrastructure. At the same time we started looking at the data sources and developing a strategy for storing the data in the efficient yet easily usable way.

Snowflake was chosen as a cloud dwh plaform, because of it's ability to control usage and cost on agranular level and ability to control access on a granular level.

dbt was chosen as a data transformation tool for the dwh, because of it flexibility, ability to generate documentation and it's approach to SQL as code.

DWH itself was designed in 3 layers to better control access to sensitive data such as PII. 

Below is schematic design of DWH developed:
<img class="dropshadowimg" src="/assets/img/2021-09-01-dwh-design.jpg" alt="DWH design schema" />

<br>
In addition to technical aspects of the data warehouse implementation, we defined and implemented a process for BI tickets and workflows.
The process is based on agile principles taking into account constant contact with a stakeholder to consider constantly changing requirements. 
In the end, we ended up working in weekly sprints to deliver value to the customers fast.
<img class="dropshadowimg" src="/assets/img/Reporting_workflow.png" alt="Reporting workflow designed" />

Steps:
1. Create a user story - the definition of metrics and dimensions is not enough to build an actionable report. At some point, a design decision will have to be made and without understanding the goal and the full picture behind the report it will be difficult to make it. Therefore this step is essential
2. Check data availability - necessary for further steps
3. Identify priorities - what are KPIs and what are supporting metrics
4. Agree on naming convention - ensure things are named consistently across the organization and names are understandable to everyone
5. Agree on deliverables - important for both sides to manage expectations and define the scope of the project
6. Add tasks to the board - helps in prioritization and to incorporate feedback
