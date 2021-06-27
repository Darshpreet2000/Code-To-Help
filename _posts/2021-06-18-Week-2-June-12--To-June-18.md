---
keywords: fastai
description: "Created Login user functionality, Created UI of Baby Assessments Phases, Support for dark mode added"
title: "Coding Period: Week 2 June 12 To June 18"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

### Creating Login User functionality

- Used flutter Bloc architecture for state management
- Used DHIS2 Auth API for authentication
- username & password is passed as Basic Auth in header in base64 encoding in API
- Users can now login using username & password in App
- Added Dark mode support
- Created config files to store dhis2 apis & id
- Added password hide/show feature

### Screen Shot
<img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2a.png" height="500" width="250">

### Created UI for Baby Assessments

Assessments are divided into multiple phases-

1. Phase 1 Assessments 0 - 90 minutes from birth

2. Phase 2 Assessments 60 - 90 minutes after phase 1

3. Phase 3 Assessments 

Categorized in 3 parts
  1. Normal
  2. Problem
  3. Danger

According to the Classification the appropriate assessment will be shown to user

### Screen Shots

<table style="width:100%">
  <tr>
   <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2f.png" height="500" width="250">
  </tr>
  <tr>
    <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2g.png" height="500" width="250"> 
  </tr>
  <tr>
   <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2h.png" height="500" width="250"> 
  </tr>
   <tr>
   <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2i.png" height="500" width="250"> 
  </tr>
   <tr>
   <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2j.png" height="500" width="250"> 
  </tr>
</table>
 


### Added Theme for Dark Mode

Toggle feature is pending but I have enabled support for dark mode

### Screen Shots

<table style="width:100%">
  <tr>
   <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2b.png" height="500" width="250">
  </tr>
  <tr>
    <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2c.png" height="500" width="250"> 
  </tr>
  <tr>
   <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2d.png" height="500" width="250"> 
  </tr>
   <tr>
   <img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week2e.png" height="500" width="250"> 
  </tr>
</table>
 

### What progress I made this week?

- Completed authentication/login functionality
- Created config files for storing API, DHIS2 Id's
- Developed UI of all three Assessments screens
- Added support for dark mode


### What I have planned to do next week?

- Register Baby screen functionality (using DHIS2 API)
- Implementing User Profile Screen functionality (using DHIS2 API)
- Making the above features work also when user is offline and sending data when user is online next time

