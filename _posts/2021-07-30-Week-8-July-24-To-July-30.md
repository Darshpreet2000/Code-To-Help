---
keywords: fastai
description: "Fetching & displaying doctor’s schedule in App with unit tests, Created Stage 5 (Discharge) with button to discharge based on conditions, Created unit test for stage 5, Made stage-4 repeatable in app after 180 minutes"
title: "Coding Period: Week 8 July 24 To July 30"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

Week 8 Of coding period is completed, I worked on adding on call doctors schedule showing screen, I created stage 5 assessments capture feature

#### Added On-Call Doctors Schedule Showing feature

Tasks

- shows list of doctor in program
- shows name, date, start time , end time of on call schedule
- shows profile image in circle
- uses cache image so that user can view image & data offline



<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/b3fd5624a771c890d7cb05bab25386ea/Screenshot_1627664147.png"  width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/1f6dece4acb34c2fa67fcfeab8d33e75/Screenshot_1627664196.png" width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/3fcac54db4ed7bf9ea9e7633f5709566/Screenshot_1627664200.png" width="300"></tr>

</table>



#### Created Stage 5 Discharge with floating button 

- Create Discharge assessments UI
- Created discharge floating action button to appear only when child is normal & 24 hours have passed
- Create model class for discharge
- Create stage 5 discharge event 
- added methods to validate , register stage 5
- added api request to mark enrollment as COMPLETED
- added method to queue api request when user is offline
- Created unit test for stage 5
- Created stage 4 variable schedule to store time




<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/d8f01395a0193ac71472fe2aec87d869/Screenshot_1627574211.png"  width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/9c841e69b35a05275f6d5277ad5b1aa1/Screenshot_1627574216.png" width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/081768c80a897660f9edc51a5b711e95/Screenshot_1627574227.png" width="300"></tr>

</table>




#### Stage 5 Unit test cases

- Throws exception if assessments are incomplete
- Marks phase-5 as complete if everything is correctly filled
- Marks child as discharged
- yields AssessmentsAdded on successful adding of phase 5
- yields AssessmentsError when assessments are incomplete while adding of phase 5 assessments


#### What progress have you made this week?

1. Fetching & displaying doctor's schedule in App with unit tests
2. Created Stage 5 (Discharge) with button to discharge based on conditions
3. Created unit test for stage 5
4. Made stage-4 repeatable in app after 180 minutes

#### What do I plan to do next week?

1. Making messaging/Notifications viewing functionality in App
2. Adding share App report bug menus in drawer
3. Preparing Documentation/Readme of Project


#### Have you had any blockers or issues that are impeding your project?

- I have completed assessments capture functionality of app, I will request feedback from mentors & will work on the same.
- I need to discuss individual/facility login feature
