---
layout: post
title: 'Automating real-time census monitoring and data cleaning for iKapaData'
author: leilei
categories:
  [agriculture, scale, automation, commcare, salesforce, telerivet, sms]
image: assets/images/myAgro1.JPG
featured: true
---

_OpenFn has saved the iKapaData team valuable time typically spent on manual data entry and cleaning processes.The real-time connection has enabled live data monitoring for the team as iKapaData survey enumerators were conducting the survey._

### iKapaData's essential work in South Africa

The census plays an important role in public administration by creating a compiled, numerical profile of South Africa. Enumerators are taught the local language and local customs in order to effectively achieve information from all households. This dataset is used as a benchmark in research and analysis for the public administration to determine policy decisions, budget decisions, and more. OpenFn enabled a system for iKapaData to ensure this delivery of accurate and timely information for the census. 

[iKapaData](http://ikapadata.com/) is a survey research and data science company with an aim to make data accessible, tangible, and actionable. For a census in South Africa, they were collecting household data using [SurveyCTO.](https://www.surveycto.com/) Each enumerator participating in the fieldwork was equipped with a tablet and an external GPS device for data collection. 

![]({{ site.baseurl }}/assets/images/farmers.jpg)

### Only problem was they did not have a way to actively monitor the enumerators' data collection. 

As enumerators collected the census data, iKapaData wanted to analyze that dataset using two reporting applications, Carto and Zoho – each with its own data model and required formats. To upload the data into the two reporting systems, iKapaData would have to rely on time-intensive manual data migration, and there was no easy way to actively monitor the census data collection. 

### How live data monitoring was eventually enabled: 

By 2017, OpenFn automation saved the iKapaData team valuable time typically spent on manual data entry and cleaning processes. Using OpenFn, iKapaData set up automated data cleaning and reporting pipelines which:
- automatically extracted data from SurveyCTO on a scheduled basis, 
- transformed that data to the appropriate reporting formats for data and geo-spatial analysis, and 
- uploaded key results to Zoho Analytics while also adding locations to a map on CartoDB to display the locations already visited by enumerators. 

The real-time connection enabled live data monitoring for the team as iKapaData survey enumerators were conducting the survey.




