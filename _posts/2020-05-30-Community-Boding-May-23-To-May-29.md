---
layout: post
---
**Searching CMS Data for Hospitals**

This week I found CMS Data which contains inpatient & outpatient procedures & charges of 3000 Hospitals. I will use these datasets , but these don’t contain complete data. They have only about 150 procedures per Hospital.

Inpatient Data [**<span class="underline">(Link)</span>**](https://data.cms.gov/Medicare-Inpatient/Inpatient-Prospective-Payment-System-IPPS-Provider/tcsp-6e99)

Outpatient Data [**<span class="underline">(Link)</span>**](https://data.cms.gov/Medicare-Outpatient/Provider-Outpatient-Hospital-Charge-Data-by-APC-CY/fmbt-qrrw)

**Preparing Project Plan for Coding Period**

I have made a detailed project plan with milestones in it. I have discussed it with my mentors. I will be making UI of complete App with Dummy Data in the first two weeks.

I have planned to scrap 2000 Hospitals Data, for which I have to save link to each hospital’s CDM to my web crawler & then process the data.

My Detailed Project Plan [**<span class="underline">(Link)</span>**](https://docs.google.com/document/d/1UItziPiwowk6QmOttp6O_d0fld5SMFaKV4xZ8dx34OQ/edit?usp=sharing) , I have to make some changes in it.

**Analyzing CDM**

I have analyzed after reading cdm of few hospitals that after processing, CDM will have three columns,

  - > Description \[Description of Procedure or Drug\]

  - > Charge \[Price of Procedure or Drug\]

  - > Category

> ◦ DRG (Diagnostic Related Group)
> 
> ◦ Pharmacy (It will contain medicines),
> 
> ◦ Standard (if no category is provided I will name it default as Standard)

**What do I plan to do next week?**

I will start making App UI with dummy data in next two weeks, I will also scrap Hospitals CDM of California State next week.
