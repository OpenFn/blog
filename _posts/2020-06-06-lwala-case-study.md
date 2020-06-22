---
layout: post
title: 'Working Towards Strengthening Healthcare in Western Kenya'
author: leilei
categories:
  [case study, lwala, kenya, ict4d, healthcare, commcare, salesforce, MoHdata]
image: assets/images/lwala1.jpeg
featured: true
---

_Using OpenFn, Lwala has not only integrated its underlying health information systems, but it has also created valuable, automated feedback loops for CHWs through its “CHW Stats” solution._

### Lwala's Mission and Vision

[Lwala Community Alliance](http://www.lwala.org) is a community-led innovator proving change is drastic and lasting when communities take charge. Based in rural western Kenya, Lwala operates in a region that faces high infant and maternal mortality rates and HIV rates almost triple that of the national average. They decided to address these challenges themselves through innovative community-led solutions designed to transform local health systems. 

As part of its holistic approach, Lwala supports an extensive network of Community Health Workers (“CHWs”) who track, screen, and refer every pregnant mother and child under 5. The longitudinal data collected by CHWs, allowing them to provide care tailored to each family and identify and manage urgent cases as quickly as possible. 

#### Lwala staff spent several hours every week managing thousands of patient records in paper forms.  

To manage patient healthcare, Lwala CHWs would receive paper-based patient records once monthly and take one week to input those records in the database. This time-intensive process resulted in significant time lags between data collection, analysis, and action. 

Lwala wanted to incorporate a mobile case management application (CommCare) to reduce the data entry lag time and to make their data more reliable and timely for CHWs. That said, Lwala didn’t have a way to automatically connect data collected via their CommCare mobile app with their central Salesforce patient database. 

#### OpenFn saves staff ~200 hours of data entry every quarter. 

To deliver real-time information exchange between its health systems, Lwala implemented Open Function to automatically integrate data between CommCare and Salesforce. Mother and child health data collected by CHWs in the field via tablet is now automatically reflected in Lwala’s central database where it can be easily analyzed by Lwala M&E and Program staff. Crucial updates made from within the database are now also automatically synced to CHWs’ mobile phones, ensuring they have the most up-to-date information possible. Read more about Lwala’s OpenFn solution [here](openfn.org/solutions). 

![]({{ site.baseurl }}/assets/images/lwala2.jpeg)

Using OpenFn, Lwala has not only integrated its underlying health information systems, but it has also created valuable, automated feedback loops for CHWs through its “CHW Stats” solution. Before OpenFn, the majority of the data collected were accessible only to health system administrators and key program users. As a result, CHWs did not usually receive regular feedback regarding their own performance, even though they are the primary data collectors. Lwala introduced “CHW Stats” to automatically share feedback with CHWs, helping them to monitor their own impact, and increase their productivity and performance. Here’s how the solution works:

1. In real-time, OpenFn syncs CommCare data collected by CHWs with Salesforce. 
2. Salesforce reports and automation summarize the data collected to update key indicator results (i.e., “total children immunized”). 
3. On a scheduled basis, a [OpenFn job](https://github.com/OpenFn/lwala/blob/master/salesforce-commcare-jobs/CHW-Stats.js) automatically forwards key CHW performance metrics back to CHW CommCare users. 
4. CHW CommCare users can regularly check these “CHW Stats” on their mobile phones for up-to-date feedback and monitor their performance for key indicators over time. 

![]({{ site.baseurl }}/assets/images/chwsnippet.png)

These feedback loops are critical to informing CHWs on key metrics (e.g., total patients reached, immunized, etc.), and they enable CHWs to better plan their services. 

#### Next steps: Adapting to COVID-19 and expanding to new provinces through partnership with the Ministry of Health

This year Lwala is expanding OpenFn to support new data collection workflows for COVID-19 healthcare protocols and partner reporting needs. In 2019, Lwala officially partnered with the Kenyan Ministry of Health (MoH) to expand its services to two new Kenyan provinces. To support this expansion, Lwala grew its OpenFn connected health system solution to integrate new CommCare tools for the MoH data collection. As MoH reporting requirements evolve, Lwala can adjust its OpenFn solution in minutes to support new data collection needs. 

In response to COVID-19, Lwala’s [Q1 report](https://lwala.org/wp-content/uploads/2020/05/Lwala-Community-Alliance-Insider-Report-Q1-2020.pdf#page=11) shows their introduction of a household screening process where CHWs will call households in advance of a patient visit to check for symptoms. While the new protocol required new training for CHWs, the underlying OpenFn-connected solution only took minutes to modify to support this new screening process. By strengthening the community-based care specific to COVID-19, Lwala is protecting health workers, interrupting the spread of the virus, and maintaining essential health services. 


Read our Medium blog [post](https://medium.com/@taylordowns2000/building-a-real-time-decision-support-tool-for-community-health-workers-75ef8a4ba520?source=---------7------------------) and [Lwala case study](openfn.org/solutions) to learn more.

