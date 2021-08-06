---
keywords: fastai
description: "Notification count, About app, Share app feature, Load more notifications functionality"
title: "Coding Period: Week 9 July 31 To August 06"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

Week 9 Of coding period is completed, I worked on adding notification count, About app, Share app feature, Load more notifications functionality

#### Notification count

I created notifications count in bottom app bar, It displays the count of new notifications in app, After fetching data from dhis2, app check if it has the message id , if it doesn't have the id then count is incremented.

When user visits the profile page then count becomes 0 as the messages are read by the user now.


<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/2b4969eaddfc0d881716bb0b56b198c1/Screenshot_1628246331.png"  width="300"></tr>
</table>



#### About app 


It displays about the project with a button to visit the project, This screen will be useful for promoting LibreHealth organization to users who are using this application.

<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/7a61c37793badc423295fa3696513231/Screenshot_1628246692.png"  width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/101b5f08043a8f1d0abacbaa8497b74f/Screenshot_1628246715.png" width="300"></tr>

</table>




#### Load more notifications
 
 When user click on load more button then it fetches the next 5 notifications, It calls api with next page number & save the data to hive storage.
 
<table>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/69eeea895126b0fb3f64f2cddb533e3f/Screenshot_1628246667.png"  width="300"></tr>
<tr align="left"><img src="https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/uploads/ea68d5171975a11660fd735f2d14ac30/Screenshot_1628247062.png" width="300"></tr>

</table>

#### Link to merge request https://gitlab.com/librehealth/incubating-projects/mhbs/lh-mhbs-eceb/-/merge_requests/24

#### What progress have you made this week?

1. New notifications count viewing on bottom bar
2.  About App, Share App, Report bug menus in drawer
3. Added Load more feature on notifications

#### What do I plan to do next week?

1. Prepare Documentation/Readme for App & how to setup 
2. Creating screen to add server url
3. Individual/facility login
4. Creating App Icon, Splash screen, Intro Slides
5. fetching program rules for classification function
6. Updating metadata for both programs
7. Finding & fixing bugs
8. Deploy to F-Droid

#### Have you had any blockers or issues that are impeding your project?

No
