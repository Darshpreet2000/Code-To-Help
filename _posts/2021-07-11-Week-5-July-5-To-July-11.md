---
keywords: fastai
description: "Classifying Baby Health, Stage - 2 Assessments Capture, Notifications showing feature, Unit testing phase - 1, Search/Sort list of babies screen"
title: "Coding Period: Week 5 July 5 To July 11"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

#### Stage 2 Assessments Capture with Classification

- Created stage-2 assessments capture with clasifying baby's health using program rules
- Health is classified in three categories (Normal, Problem, Danger)
- App takes all data entered by user in stage 2 & then evaluate program rules for classifying health
- After classifying health the color of assessments screen changes according to the category



#### Stage 2 Notifications showing feature

- Used [awesome_notifications](https://pub.dev/packages/awesome_notifications) package for displaying notification
- Displaying scheduled notifications reminder if user has not completed assessments
- Displaying notification on stage assessments opening
- Created Offline Notification showing functionality
   1. Showing notification when baby is registered to complete phase -1  assessments
   2. If user forgets to do phase 1 assessment then reminding by notification again after 60 minutes
   3. Notification feature works offline using scheduled notification featur
   4. Package used for showing notification https://pub.dev/packages/awesome_notifications


### Screenshots of notifications


<table style="width:100%">
  <tr>
<img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/494aaa7f344e5e1bf33d0014ad4056d5/Screenshot_1625675204.png" width="300"> 
 </tr>
  <tr>
<img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/ff8b3c74f1478fcce18f16830c6c3689/Screenshot_1625674080.png" width="300">  
</tr>
  <tr>
<img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/cf060d2501960c3aa0b6a9dbaa7fb953/Screenshot_1625674090.png" width="300">
  </tr>
</table>
#### Unit testing assessments bloc, client, repository, phase-1
Test Cases 

* Flutter Assessment BloC test
   * Test Cases
   * yield AssessmentsInitial on successful fetching of data
   * yields AssessmentsError on unsuccessful fetching of data
   * yields AssessmentsAdded on successful adding of phase 1
   * yields AssessmentsError when ward name is empty while adding of phase 1 assessments
   * yields AssessmentsError when assessments are not completed while adding of phase 1 assessments
<br>

* AssessmentsRepository testing
  * Test Cases
  * Throws exception if wardname is empty
  * Throws exception if assessments are incomplete
  * Marks phase-1 as complete if everything is correctly filled
  * Adds stage-1 assessments if list is empty
<br>

* Assessment Client Test
  * Test Cases
  * returns response with 200 code on successful fetching of assessments
  * throws fetch data exception on no internet connection



#### Searching & sorting functionality on list of babies screen

#### Sort List of babies by
   * Time (Birth Time) 
   * Status ( Classificiation - Normal, Problem, Danger ) (Danger & Problem have high priority)
   * Location ( Ward Name)




| By Birth Time| By Status |  By Location |
| ------ | ------ | ------ |
| ![Screenshot_1625831445](https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/fc83bc45c8d404a4dd52adeb89377f93/Screenshot_1625831445.png)| ![Screenshot_1625831527](https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/ee65c0679d6c38b6ad4d9904be912437/Screenshot_1625831527.png)| ![Screenshot_1625831549](https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/ea78d27d5a92f6cddbba69be7720eb9e/Screenshot_1625831549.png)|

#### Search List of babies by mother's name



| Search Oni| Search test |
| ------ | ------ |
| <img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/48bbcab698dbc6610f1556f6c41b2cd5/Screenshot_1625831565.png" width="300">| <img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/65c9af1c4bc3a95455b5eade5abfdda1/Screenshot_1625831575.png" width="300">|


#### What progress have you made this week?

* Adding Search, Sort Functionality in List Of Babies screen  
* Unit Testing Assessments Bloc, Client, Repository, Phase 1
* Created Phase-1 Notifications showing functionality
* Created Phase-2 Assessments Capture with notifications 

#### What do I plan to do next week?

* Phase - 3, 4  assessments capturing functionality
* Showing summary in Home Screen
* Developing settings screen of app
* Unit Testing phase - 2 , 3 , 4
