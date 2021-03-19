---
layout: about 
---

# About Me
I came to the digital analytics world with background in electronics, basics in Assembler language and some management experience from my time in the Air Force. Since then I worked on a lot of projects ranging from analysis of marketing campaigns to migration of data warehouse and built quite a portfolio of successful [projects](\portfolio\). Nonetheless, I'm always looking for new technologies to try and new projects to work on.

Professionally I've always been guided by these 4 principles:

{:#principles}
- **Accountability** - Taking responsibility and behaving ethically and transparently
- **Quality** - Focusing on customer satisfaction by delivering better than expected results 
- **Agility** - Welcoming and adjusting to changes to make progress continuously
- **Impact** - Focusing on things that matter and generate value



<br/>

# Career


### Experteer GmbH, Munich 
* Design and implementation of ETL solutions to enrich DWH with new data
* Administration and maintenance of data warehouse (SQL Server)
* Successful migration from VBA scripts to extraction of data with Python to increase data quality
* Led the team in migration of company reporting from Excel to Power BI
* Automated report updates using python, Google Apps script and SSIS
* Prepared and presented analysis to the top management in various business functions
* Successful management of digital analytics and tracking projects (Google Tag Manager and Google Analytics)
* Creation and implementation of tracking, reporting and analysis concepts
* Technical & Backlink SEO audit (Screaming Frog, DeepCrawl, Sistrix, Buzzstream)


### InterNations, Munich
* Preparation of ad-hoc analysis and reports using MySQL database
* Optimization of reports and VBA macros
* Creation and optimization of ETL processes (Pentaho spoon)


###  Israeli Air Force, Israel
* Department management
* Responsible for information security and quality control in the department
* Installation and maintenance of the communication and navigation equipment for the aircraft
* Responsibility for expansive equipment and excellent quality of work

<br/>

# Interests
I am interested in technology trends.  
I'm not afraid to learn languages, but I enjoy using Python.  
I like to automate and reduce annoying things.  

<br/>

# Technologies

<table>
{% capture tags %}
{% for tag in site.tags %}
{{ tag[1].size | plus: -10000 }}###{{ tag[0] | replace: ' ', '##' }}###{{ tag[1].size }}
{% endfor %}
{% endcapture %}
{% assign sorted_tags = tags | split: ' ' | sort %}


{% tablerow sorted_tag in sorted_tags  cols:3 limit:15 %}
{% assign items = sorted_tag | split: '###' %}
{% assign tag = items[1] | replace: '##', ' ' %}
{% assign count = items[2] | plus: 0 %}
{% if count > 5 %}
{% assign size = 5 %}
{% else %}
{% assign size = count %}
{% endif %}
<span class="tag-size-3">
<a class="tag-link" href="/tags/{{ tag | slugify }}" rel="tag">{{ tag | replace:'-', ' ' }}</a> 
</span>


{% endtablerow %}
</table>

