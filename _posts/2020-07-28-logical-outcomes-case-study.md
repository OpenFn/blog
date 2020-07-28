---
layout: post
title: 'Automating CSV File Uploads to DHIS2 to Connect and Clean Siloed Datasets'
author: leilei
categories:
  [
    case study,
    data cleaning,
    dhis2,
    Logical Outcomes,
  ]
image: assets/images/logicaloutcomes.jpg
featured: false
---

_OpenFn can connect any CSV file uploaded to an online location–helping organizations like Logical Outcomes automatically connect all siloed data sources to DHIS2._

### DHIS2 is typically used on a national scale and summarizes data from multiple data sources, which are collected across a range of different tools.

While DHIS2 offers some out-of-the-box integration options, organizations using external data collection tools must either integrate with the [DHIS2 web API](https://docs.dhis2.org/2.22/en/developer/html/ch01.html) or [import data](https://docs.dhis2.org/2.22/en/user/html/ch21s02.html) from XLS files. Because Excel is still a core data collection tool for many organizations, this XLS import process is necessary–but typically very time-consuming, prone to human error, and difficult to enforce data quality standards.

### [Logical Outcomes](https://www.logicaloutcomes.net/) is a non-profit consultancy helping organizations, including [CARE](https://www.care-international.org/) and [The Nature Conservancy](https://www.nature.org/en-us/about-us/who-we-are/?intc=nature.tnav.about), to implement and effectively leverage DHIS2 for enhanced data management. 

Every project Logical Outcomes consultants typically spent several hours on data migration tasks to just move their clients’ data from Excel to DHIS2. This process was not only time-consuming, but it was also prone to human errors and difficult to check for duplicate records in DHIS2.

### To speed up data migration and better ensure data quality for its clients, Logical Outcomes used OpenFn to automatically clean CSV data and run duplicate-checks with DHIS2 before uploading new records.

Whenever Logical Outcomes uploads a new CSV file to OpenFn.org, OpenFn parses and cleans the data, checks for duplicates, and connects with the DHIS2 web API to import new Tracked Entity, Enrollment, and Event records, as directed by data upload “rules” defined in OpenFn _jobs_ (or automation “scripts”). If any existing records are found, OpenFn will _update_ the existing DHIS2 records.  If there are any data upload errors, OpenFn will send error notifications immediately so that staff can address any data issues before re-uploading. 

While typically used for live integration and data streaming between applications, OpenFn can connect any CSV file uploaded to an online location–helping organizations like Logical Outcomes _automatically_ connect all siloed data sources to DHIS2.

Is your organization using DHIS2 and considering how to integrate data sources? Read how SwissTPH uses OpenFn for real-time DHIS2 integration with CommCare, or contact our team at admin@openfn.org to learn more about DHIS2 integrations.

