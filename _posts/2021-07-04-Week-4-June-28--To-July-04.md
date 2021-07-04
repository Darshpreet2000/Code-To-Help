---
keywords: fastai
description: "Stage - 1 Assessments Capture, fetching list of babies from dhis2, User Profile Screen functionality"
title: "Coding Period: Week 4 June 28 To July 4"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

### Stage 1 Assessments Capture Functionality

- Fetching & Capturing Stage - 1 Assessments , with this feature user is able to view the captured assessments & also capture the assessments and push the data to DHIS2.
- This works offline also, data is sent to server when user refreshes on having internet next time
- Created a BLoC to handle assessments 
- Created Stage - 1 model class which parses and converts to JSON format for parsing and converting data
- added required ID's in static variables in dhis2_config.dart file
- created a client to send data, created a repository to handle data from client


### Fetching list of babies enrolled in program

- Created a BLoC for fetching list of babies enrolled in a program
- Creating a client & repository class for fetching & saving data locally
- Sorting the list by time to categorize recently & past registered babies
- On Tap of baby list item the app opens assessments screen & start fetching assessments
- List item color changes with classification of baby - Danger (Red), Problem (Yellow), Normal (Green)

[Merge Request Link](https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/-/merge_requests/10) 


### User Profile Screen Functionality

- Fetching list of users notification from dhis2
- saving data in hive storage after fetching item
- fetching & displaying the notification date & time for each notification

[Merge Request Link](https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/-/merge_requests/9) 


### Localized strings in assessments phases UI

- All strings used in assessments phases UI are now localized
- localized strings are saved in app_en.arb file 

[Merge Request Link](https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/-/merge_requests/8) 


### What progress have you made this week?

* Implemented User Profile Screen functionality  
* Implemented fetching list of babies from dhis2 & displaying in screen
* Cache the data after fetching from dhis2
* localized strings in assessments phase
* Phase 1 assessments capturing functionality

### What do I plan to do next week?

* Phase - 2, 3, 4  assessments capturing functionality
* Adding Search, Sort Functionality in List Of Babies screen
* Adding sort functionality , settings UI, activity logs in profile screen
* Update functionality in profile screen
