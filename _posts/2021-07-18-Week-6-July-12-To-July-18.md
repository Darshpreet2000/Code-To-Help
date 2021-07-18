---
keywords: fastai
description: "Settings drawer, Stage - 3 Assessments Capture functionality, Stage- 2 Unit testing, showing summary in home screen"
title: "Coding Period: Week 6 July 12 To July 18"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

#### Settings drawer to toggle settings with unit test

- Created end drawer to toggle settings 
- User can toggle notifications, notifications sound, dark mode
- The settings done by user are saved instantly in storage and changes are made according to it
- Wrote unit test for settings bloc with test cases
      1. yields SettingsState on toggle of dark mode
      2. yields SettingsState on change of notifications sound
      3. yields SettingsState on toggle of notifications

<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/257337fc39bccc50b11aec0f1b59b0a8/Screenshot_1626603574.png" width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/7c2fd97371e106fbf70a8386e25bc83e/Screenshot_1626603578.png" width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/f3a56b728e9506dbbcdd85d9699817c1/Screenshot_1626603588.png" width="300"></tr>

</table>


#### Stage 3 Assessments Capture functionality

- Stage 3 has 3 types (normal, problem, danger)
- If a baby is classified as any type then that type of stage 3 assessments get added in app

### Video GIF showing stage - 2 with classification functionality

- background turns red on danger 
- background turns yellow on problem
- background turns green on normal 

<table>
<thead>
<tr class="header">
<th align="left">Classifying as Danger after stage 2 assessments</th>
<th align="left">Classifying as Problem after stage 2 assessments</th>
</tr>
</thead>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/7079f679b2ecd23675fb4af30d41b43e/danger.gif" width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/224cdc2a57c09e671e043e0aa2d1a633/problem.gif" width="300"></tr>

</table>


#### Stage 2 Unit testing

Test Cases for stage-2
-  Throws exception if assesments are done before 60 mins from birth
-  Throws exception if wardname is empty
-  Throws exception if assessments are incomplete
-  Marks phase-2 as complete if everything is correctly filled
-  Adds stage-2 assessments if list is empty

Test Cases for Classification Repository
- if temperature < 95.5 or > 99.5 then classifies as danger
- if severe jaundice or fast breathing then classifies as danger
- if weight < 2000 & poor feeding then classifies as problem
- if everything is normal then classifies as normal

#### Showing summary of 24 hours in home screen

To show summary of 24 hours, We need to use lastUpdatedDuration=1d (1 day) as parameter in API to fetch all the events happened within 24 hours.

This has 3 types

- Admitted Count - Check Status = ACTIVE & Enrollment Date yesterday
- Discharged - Check Status = COMPLETE 
- High Risk  - For each TEI (Baby) this needs to be counted by parameter classification



#### What progress have you made this week?

* Phase - 3, 4  assessments capturing functionality
* Showing summary in Home Screen
* Developing settings screen of app
* Unit Testing phase - 2 

#### What do I plan to do next week?

-  Adding On-Call Doctors Viewing Functionality in App
- Completing Notification screen (Risk Assessment, Monitoring Alerts Tab)
- Phase - 3,4 Unit testing

