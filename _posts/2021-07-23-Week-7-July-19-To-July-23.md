---
keywords: fastai
description: "Added On-Call Doctors Viewing Functionality in App, Completed Notification screen (Risk Assessment, Monitoring Alerts Tab), Phase - 3,4 Unit testing"
title: "Coding Period: Week 7 July 19 To July 23"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

Week 7 Of coding period is completed, I worked on adding on call doctors viewing feature, I completed notifcation showing functionality on risk assessments and monitoring alerts

#### Added On-Call Doctors Viewing Functionality in App with Unit tests

- Fetching events from on call doctors program
- displaying on call doctors
- displaying images with cache
- saving the list to local storage

###### Unit tests

- yield OnCallDoctorLoaded on successful fetching of data
- yields OnCallDoctorLoaded on unsuccessful fetching of data by getting from hive
- returns response with 200 code on successful fetching of on call doctors
- throws fetch data exception on no internet connection


<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/6074243f3d0f264958faf54ecd311cda/Screenshot_1626859610.png"  width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/a4bdcd27fc4fcb94c18930f121d3d9e0/Screenshot_1626859590.png" width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/5751fe9fcdc74830adaf28446bc116f1/Screenshot_1626859593.png" width="300"></tr>

</table>


GIF Showing on Call Doctors slider

<img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/042c0945a9df7bd51c64522b2c2d16eb/on_call_doctors.gif" width="300">

#### Completed Notification screen (Risk Assessment, Monitoring Alerts Tab) with Unit tests


- Created notification screen bloc
- Created repository with methods to get risk assessments and monitoring alerts
- on tap of the list item the child assessments are opened

#### Unit tests
- Flutter Notifcation BloC test
- Test Cases
- yield NotificationLoaded on Fetch Nofitication Of Babies
- Flutter Notifcation Repository test
- Test Cases
- Risk Assessments Test cases
- status changed normal to danger
- status changed problem to danger
- status changed normal to problem
- status changed danger to problem
- Monitoring Alerts Test cases
- stage-4 assessments next



<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/b51a91d3d9d5e6a0d4cefea170cb5f5f/Screenshot_1626954594.png"  width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/230caf2b0f3d400c2b2fad7016c0c411/Screenshot_1626954596.png" width="300"></tr>

</table>




#### Unit tests Phase 4

##### AssessmentsRepository Test Cases
- Throws exception if assesments are done before 180 mins from birth
- Throws exception if assessments are incomplete
- Marks phase-4 as complete if everything is correctly filled
- Adds stage-4 assessments if list is empty

##### AssessmentsBloc Test Cases
- yields AssessmentsAdded on successful adding of phase 4
- yields AssessmentsError when assessments are incomplete while adding of phase 4 assessments

#### Phase 3 Assessments Unit testing 
 Test Cases
- Throws exception if Stage3 Normal assessments are incomplete
-  Throws exception if Stage3 Problem assessments are incomplete
-  Throws exception if Stage3 Danger assessments are incomplete
- Marks Stage3 Normal as complete if everything is correctly filled
-  Marks Stage3 Problem as complete if everything is correctly filled
-  Marks Stage3 Danger as complete if everything is correctly filled
-  Adds Stage3 Normal assessments if list size is 2 and classification is normal
-  Adds Stage3 Problem assessments if list size is 2 and classification is problem
-  Adds Stage3 Danger assessments if list size is 2 and classification is danger

##### Bloc Test
- yields AssessmentsAdded on successful adding of phase 3
- yields AssessmentsError when assessments are incomplete while adding of phase 3 assessments

#### What progress have you made this week?

- Added On-Call Doctors Viewing Functionality in App
- Completed Notification screen (Risk Assessment, Monitoring Alerts Tab)
- Phase - 3,4 Unit testing

#### What do I plan to do next week?

1. Fetching & displaying doctor's schedule in App with unit tests
2. Making messaging/Notifications viewing functionality in App with unit tests
3. Creating share App report bug features
4. Creating Stage 5 (Discharge) Stage with unit tests

