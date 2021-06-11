---
keywords: fastai
description: "Developing UI of Register Baby Screen & Making App Drawer"
title: "Coding Period: Week 1 June 07 To June 11"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

### Developing UI of Register Baby Screen

I worked on creating UI of register baby screen, I have used the following packages

- Flutter Customizable Slider for weight, temperature input [(Link)](https://pub.dev/packages/syncfusion_flutter_sliders)

- Flutter Date Time Picker to pick baby's birth date & time [(Link)](https://pub.dev/packages/flutter_datetime_picker)

- Flutter Bloc Architecture to handle state management [(Link)](https://pub.dev/packages/flutter_bloc)

I have created toggle buttons for baby's information input such as gender, mode of delivery etc. These toggle buttons uses boolean variable for their state management. 

I have created a model class for storing Baby's health information, This class's object is created & data is filled when user enter's data is register baby's screen.


### Creating Navigation Drawer in App

I Added a navigation drawer in app, It has the following items & header with LibreHealth's Logo.
- Doctor’s Schedule
- Messaging
- About
- Share App
- Report Bug


### Screen Shots

<img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week1a.png" height="500">

<img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week1b.png" height="500">


<img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/images/week1c.png" height="500">

### What progress I made this week?

- Developed UI of Register Baby Screen
- Created Sliders for weight, temperature etc.
- Created Model Class for storing Baby's Information
- Created Bloc for register baby screen
- Created App Drawer with items ( Doctor’s Schedule, Messaging, Share App, Report Bug)


### What I have planned to do next week?

- Developing Assessments Screen UI for all stages 
- Using Sliver App Bar for floating app bars
- Adding Dark Mode in App
