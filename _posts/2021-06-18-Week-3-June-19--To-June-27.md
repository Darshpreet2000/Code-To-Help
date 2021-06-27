---
keywords: fastai
description: "Internationalized app, added metadata, performed unit testing for authentication, created register baby functionality"
title: "Coding Period: Week 3 June 19 To June 27"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
layout: post
---

### Internationalized Flutter app by adding support for other languages

Created .arb (Application Resource Bundle) file which contains key-value pair strings, I localized all the string text using till now in app.
For now I have added translations for 3 languages only


### Added metadata of ECEB & on call doctors programs

DHIS2 provides a metadata repository containing metadata packages with various content. A metadata package is a DHIS2-compliant JSON document which describes a set of metadata objects. I exported this metadata for the ECEB & On call doctors program. Users who will use this app will need to import this metadata in their dhis2.

### Unit testing for authentication screen

Unit tests are handy for verifying the behavior of a single function, method, or class. I created unit test for the auth functionality.

Test Cases for Hive Storage
1. User loggedIn return true
2. Not LoggedIn return false

Flutter BloC test cases
1. yield AuthenticationLoaded on successful login
2. yield AuthenticationError on unsuccessful login

Auth Client Test Cases
1. response code 200 - successful login
2. response code 401 - unauthorized (wrong credentials)
3. Socket Exception - no internet connection

### Register Baby screen functionality

* Baby able to get registered using app & their data is stored using api in DHIS2.
* This feature works offline also, data is synced when user is online next time
* Created a refresh bloc for state management
* Added Snackbars for showing info related to syncing
* stored the list in hive storage


### What progress I made this week?
- Internationalized Flutter app by adding support for other languages
- Added metadata of ECEB & on call doctors programs
- Unit testing for authentication screen
- Register Baby screen functionality (using DHIS2 API)

### What do I plan to do next week?
- Implementing User Profile Screen functionality
- Baby Health Assessments Capture Functionality
- Fetching List Of Babies screen in App using API
