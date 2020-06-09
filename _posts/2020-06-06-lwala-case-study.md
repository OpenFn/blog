---
layout: post
title: 'Working Towards Strengthening Healthcare in Western Kenya'
author: leilei
categories:
  [lwala, kenya, ict4d, healthcare, commcare, salesforce, MoHdata]
image: assets/images/lwala1.jpeg
featured: true
---

_Lwala implemented OpenFn in 2016 to automatically pass data between CommCare and Salesforce, providing CHWs with real-time data to inform healthcare  protocols, highlight priority clients, and identify which patient to visit next._

### Lwala's Mission and Vision

[Lwala Community Alliance](http://www.lwala.org) is a community-led innovator proving change is drastic and lasting when communities take charge. They are based in rural western Kenya, where there are high infant and maternal mortality rates and HIV rates almost triple that of the national average. Lwala decided to address these challenges themselves through innovative community-led solutions designed to transform health systems. 

As part of its holistic approach, Lwala supports an extensive network of Community Health Workers (CHWs) who track, screen, treat and refer every pregnant mother and child under 5. The longitudinal data collected by CHWs supports their provision of healthcare at the household, allowing them to provide care tailored to each family and identify and manage urgent cases as quickly as possible. 

### However, managing thousands of patient records in paper forms was wasting valuable staff time. 

To manage patient healthcare, Lwala CHWs would receive paper-based patient data once a month and take another week to input that data, losing valuable staff time and increasing time lags between data collection, analysis, and action. They wanted to incorporate a mobile case management application (CommCare) to reduce the lag time required for data entry from paper forms and to make their data more reliable and timely for CHWs. That said, Lwala didn’t have a way to automatically connect data collected via CommCare, the mobile app, with their central Salesforce-based patient database. 

![]({{ site.baseurl }}/assets/images/lwala2.jpeg)

### Lwala decided to implement OpenFn in 2016. 

OpenFn facilitates bi-directional data flows between CommCare and Salesforce, enabling Lwala to use Salesforce analytics to summarize data across CHWs, as well as create feedback loops for CommCare mobile users. On a scheduled basis, Lwala pushes key performance metrics back to CHW CommCare mobile users via OpenFn. Leveraging the OpenFn CommCare language-package, this "CHW Stats" job accesses CommCare's submission API to submit a CommCare form and thereby share key performance metrics calculated in Salesforce with the CHWs, using CommCare mobile. This provides CHWs with real-time data to inform healthcare  protocols, highlight priority clients, and identify which patient to visit next. Lwala CHW supervisors can then review these stats on mobile to monitor key performance metrics such as number of households reached, number of home delivers, etc. 

Mother and child health data collected by CHWs via mobile phone is now automatically reflected in Lwala’s patient database where it can be easily analyzed by Lwala M&E staff. Patient updates entered in the database are now also automatically synced back to mobile phones, ensuring CHWs always have access to the most up-to-date information. This OpenFn-powered connected health system saves the organization about 205 hours/quarter in data entry time. It has also made CHWs’ jobs easier by getting them the crucial information they need, faster. Lwala didn’t stop there. 

### The next steps: Expanding to new provinces through partnership with the Ministry of Health.

In 2019, Lwala expanded its efforts to two new Kenyan provinces through a partnership with the Ministry of Health, reaching a population of 90,000. To support this expansion, Lwala expanded its OpenFn solution and integrated new CommCare tools for MoH data collection. With that in place, Lwala was able to grow its team of CHWs who are now five times more likely to be aware of danger signs in pregnancy and early infancy compared to existing health volunteers (Lwala Community Alliance, 2019 Annual Report). 


Read our Medium blog [post](https://medium.com/@taylordowns2000/building-a-real-time-decision-support-tool-for-community-health-workers-75ef8a4ba520?source=---------7------------------) to learn more.

