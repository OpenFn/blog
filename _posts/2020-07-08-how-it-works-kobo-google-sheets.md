---
layout: post
title: 'OpenFn Blueprint: How I Integrated Kobo Toolbox and Google Sheets in 5 Minutes for Real-Time Health Facility Monitoring'
author: aleksa
categories:
  [how-to, ict4d, automation, Kobo Toolbox, Google Sheets]
image: assets/images/kobo-toolbox.png
featured: true
---
_With the free OpenFn plan, you can integrate up to 100 Kobo surveys per month with any data system (Google Sheets, DHIS2, MySQL MongoDB, Salesforce, and more)._

**This is the first post in the OpenFn “How To” series. Read on to learn more about OpenFn:**
- Data integration
- Monitoring systems
- Data cleaning
- Kobo Toolbox and Google Sheet connections

Recently I’ve been working on several integration projects connecting Kobo Toolbox with DHIS2 and other data repositories. 

**The use case: As a M&E team member, I want to integrate my survey collection tool to my data repository, so that I can monitor and visualize data collected in real-time.**

Most recently, I helped The Population Council in Kenya integrate Kobo Toolbox with Google Sheets for real-time monitoring of possible serious bacterial infection (PSBI) activities in health facilities across Kenya (read more about the initiative here). Pop Council leveraged Google’s free data visualization tools to configure a monitoring dashboard, but needed data integration to turn this into a live, dynamic dashboard. 

While there is an available Google script that syncs Google Sheets with Kobo on-demand, this still requires someone to click a button every time you want refreshed data. So here’s how I implemented automated data integration on OpenFn...

### Step 1. Tools - Connect Kobo Toolbox to OpenFn (see instructions here), and register your Google credentials.
I’m a big fan of Kobo Toolbox–an open-source data collection tool based on OpenDataKit (ODK). It’s an NGO favorite, quick to configure, free, well supported, and has a fairly robust data publishing REST Service feature. Within minutes, you can set up data forwarding so that Kobo survey submissions are automatically forwarded to OpenFn. 

To connect with Google Sheets, create a new OpenFn “Credential” for your Google Account. 
[screenshot]

### Step 2. Trigger - Determine what should prompt the data sync and create a new OpenFn “Trigger." 
Triggers are typically event- or timer-based. In this case, every time Pop Council submits a new “PSBI” survey, I want to send that data to my connected Google Sheet. So I used the Kobo form name to create a new “Message Filter” trigger in OpenFn. 
[screenshot] 

### Step 3. OpenFn Job - Create a new job to send the Kobo data to Google Sheets.  
Leveraging language-googlesheets (OpenFn’s Google Sheets “adaptor”), I created a new job to automatically sync the Kobo data with Google Sheets. Here’s how:
1. Create a new job using the Google Sheets adaptor and a new Credential linked to your Google account.
[screenshot]
2. Copy and paste the below job snippet ([also found here]).
[code snippet]
3. Edit the job to include the `spreadsheetId` and to specify which Kobo questions you want to send to the connected GoogleSheet.
[code snippet]
4. Save and turn “on” the OpenFn job to process data automatically, as soon as it hits your OpenFn Inbox.
 
**Bonus!** If you want to automatically clean your Kobo data before it syncs with Google Sheets, try adding some basic JavaScript into your job. For example: 
[code snippet] 

### Step 4. Action - Watch the Kobo data sync automatically and start analyzing! 
Test the integration by submitting a new Kobo survey. As soon as the survey is submitted, Kobo will forward it to your OpenFn Inbox, triggering your new job to run. OpenFn will then clean and send the Kobo data to your connected Google Sheet–automatically and in real-time! 

**With the free OpenFn plan, you can integrate up to 100 Kobo surveys per month with any data system (Google Sheets, DHIS2, MySQL MongoDB, Salesforce, and more).**

Questions? Post on the OpenFn community for help, tips, and tricks. Hoping to integrate other data collection tools? Check out OpenFn Docs to learn more, or explore our Apps page. 

Happy integrating! 
