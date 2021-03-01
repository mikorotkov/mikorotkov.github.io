---
layout: about 
---

# About Me
I came to the digital analytics world with background in electronics, basics in assembly language and some management experience from my time in the air force. Since then I worked on a lot of projects ranging from analysis of marketing campaigns to migration of data warehouse and built quite a portfolio of successful [projects](\portfolio\). Nonetheless, I'm always looking for new technologies to try and new projects to work on.

Professionally I've always been guided by these 4 principles:

{:#principles}
- **Accountability** - Taking responsibility and behaving ethically and transparently
- **Quality** - Focusing on customer satisfaction by delivering better than expected results 
- **Agility** - Welcoming and adjusting to changes to make progress continuously
- **Impact** - Focusing on things that matter and generate value



<br/>

# Career


### Experteer GmbH, Munich (2016/04 ~ )
* **Senior Business intelligence manager** (2020/02 ~ )
  * Successfully designed and implemented ETL solutions
  * Administration and maintenance of data warehouse
  * Oversee the migration of data from legacy systems to new solutions
* **Business Intelligence Manager** (2018/02 ~ 2020/02)
  * Successfully led the team in migration of company reporting from Excel to Power BI
  * Automated update for multiple marketing reports using python, Google Apps script and SSIS
  * Prepared and presented analysis to the top management in various business functions
* **Web Analytics Manager** (2016/10 ~ 2018/02)
  * Successful management of digital analytics and tracking projects
  * Provided top management with analysis and insights to improve decision making
* **SEO Intern** (2016/04 ~ 2016/10)
  * Creation and implementation of tracking, reporting and analysis concepts
  * Technical & Backlink SEO audit (Screaming Frog, DeepCrawl, Sistrix, Buzzstream)


### InterNations, Munich (2015/09 ~ 2016/03)
* **Business Intelligence Intern**
  * Preparation and optimization of ad-hoc and other reports using MySQL database
  * Creation and optimization of ETL processes (Pentaho spoon)


###  Israeli Air Force, Israel (2007/05 ~ 2012/05)
* **Team Manager** (2010/05 ~ 2012/05)
  * Department management
  * Responsibility for information security and quality control in the department
* **Communication and Navigation Technician** (2007/05 ~ 2010/05)
  * Installation and maintenance of the communication and navigation equipment for the aircraft
  * Responsibility for expansive equipment and excellent quality of work

<br/>

# Interests
I am interested in technology trends.  
I'm not afraid to learn languages, but I enjoy using Python.  
I like to automate and reduce annoying things.  

<br/>

# Skills
{% assign tags = site.tags | sort %}
{% for tag in tags %}
 <span class="site-tag">
    <a href="/tags/{{ tag | first | slugify | capitalize }}/"
        style="font-size: {{ tag | last | size  |  times: 4 | plus: 80  }}%">
            {{ tag[0] | replace:'-', ' ' }} ({{ tag | last | size }})
    </a>
</span>
{% endfor %}