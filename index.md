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

<table>
{% assign tags = site.tags | sort %}
{% capture site_tags %}{% for tag in site.tags %}{{ tag[1].size }}#{{ tag | first | downcase }}#{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tag_hashes = site_tags | split:',' %}


{% tablerow hash in tag_hashes  cols:3 limit:10 %}
  {% assign keyValue = hash | split: '#' %}
  {% capture tag_word %}{{ keyValue[2] | strip_newlines }}{% endcapture %}

  <span class="site-tag">
    <a href="/tags/{{ tag_word | first | slugify | downcase }}/"
        style="font-size: {{ site.tags[tag_word].size  |  times: 4 | plus: 80  }}%">
            {{ tag_word | replace:'-', ' ' }} ({{ site.tags[tag_word].size  }})
    </a>
</span>

{% endtablerow %}
</table>

# Test

<table>
{% capture tags %}
{% for tag in site.tags %}
{{ tag[1].size | plus: -10000 }}###{{ tag[0] | replace: ' ', '##' }}###{{ tag[1].size }}
{% endfor %}
{% endcapture %}
{% assign sorted_tags = tags | split: ' ' | sort %}


{% tablerow sorted_tag in sorted_tags  cols:3 limit:10 %}
{% assign items = sorted_tag | split: '###' %}
{% assign tag = items[1] | replace: '##', ' ' %}
{% assign count = items[2] | plus: 0 %}
{% if count > 5 %}
{% assign size = 5 %}
{% else %}
{% assign size = count %}
{% endif %}
<span class="tag-size-{{ size }}">
<a class="tag-link" href="/blog/tag/{{ tag | slugify }}" rel="tag">{{ tag | replace:'-', ' ' }}</a> ({{ count }})
</span>


{% endtablerow %}
</table>

