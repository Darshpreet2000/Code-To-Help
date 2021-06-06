---
keywords: fastai
description: "Getting Ready For Coding Period"
title: "Community Bonding Period June 1 to June 6"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

## Community Bonding Period June 1 to June 6

Coding period is about to begin tomorrow & I have done preparations to start coding, During this week I had completely set up DHIS2 with program rules/Stages

Few thing I want to Discuss

### Baby Classification Logic

Earlier I thought to do Classification in app only , but now I learned about program rules which run automatically and can classify baby easily, Moreover these rules are very much configurable so users can configure these according to their requirements

Currently I used ECEB Action plan to classify Baby's health in 3 categories - Normal/Problem/Danger

Example of Classification Logic For Danger

`#{ECEB_Severe_Jaundice} || #{ECEB_Assess_Temperature}<= 35.5 || #{ECEB_Assess_Temperature} >= 37.5  || #{ECEB_Weight} < 1500 || #{ECEB_Chest_Indrawing} ||#{ECEB_Not_Feeding} || #{ECEB_Fast_Breathing} || #{ECEB_Convulsions}`

If any of the above condition is true then the health is in danger.

The program rule has an acion - It classifies health by filling data element ECEB_Classification after evaluating the above expressions.

### Creating an Initial Screen to fetch all data elements/program ids from dhis2

For doing API call related to a program/event we need its unique id beforehand, As these ids are not constant on every DHIS2 , I need to first design a screen which fetches all the variables/Stage/Programs ID from the dhis2. Then the user will be able to use the app.

### On Call Doctor’s Program

This is an Event Program, Doctor’s schedule is added as an event with data elements name, date, start time, end time, Doctor’s Image.

<img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/on_call_doctors.png" width="60%"  > 




### What progress I made this week?

- Created program rules for Normal/Problem/Danger
- Created On Call Doctor’s Program
- Created Stage 4 & Stage 5 in DHIS2 & modified previous stages according to ECEB action plan

### What I have planned to do next week?

- Developing Register baby screen UI
- Developing Assessments Screen UI of App
- Adding Dark Mode in App
- Adding navigation drawer in app with menus ( Doctor’s Schedule, Messaging, Share App, Report Bug)
