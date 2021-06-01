---
layout: post
---
## Reading Documentation Of Flutter Packages

In the second week of community bonding, I read documentation of Flutter packages such as **flutter\_map** [**(Link)**](https://pub.dev/packages/flutter_map) which I will use to display OSM (Open Street Map ) in the app. I read its implementation from examples shown.

I read about Flutter **GeoJSON** package which I will use to read geojson output from the Overpass API response.

**location** package **[(Link)](https://pub.dev/packages/location)** It is another package which I will use to get current location of User.

I will get latitude & longitude of user which I will use in Overpass API to get Nearby Hospitals

## Using Overpass API to retrieve Nearby Hospitals

I learned to use Overpass API to show nearby Hospitals, I have used Overpass turbo to test my API calls.

Overpass API uses a Query Language to get data from its Server. I read its documentation carefully. [**(Here)**](https://wiki.openstreetmap.org/wiki/Overpass_API)

I read its various examples, I will summarize my points here

### Base URL 

https://lz4.overpass-api.de/api/interpreter

### **Around**

Around allows you to get all nodes near one or more given nodes.

Example

[around:<span class="underline">1</span>000](https://lz4.overpass-api.de/api/interpreter?data=[out:json];%20\(%20node\(around:8000,39.435200,%20-74.605448\)["amenity"="hospital"];%20way\(around:8000,39.435200,%20-74.605448\)["amenity"="hospital"];%20\);%20/*added%20by%20auto%20repair*/%20\(._;\>;\);%20/*end%20of%20auto%20repair*/%20out%20body;%20\>;) in area of 1 Km.

Need to pass current location coordinates

[(around:<span class="underline">1</span>000,39.435200,%20-74.605448)](https://lz4.overpass-api.de/api/interpreter?data=[out:json];%20\(%20node\(around:8000,39.435200,%20-74.605448\)["amenity"="hospital"];%20way\(around:8000,39.435200,%20-74.605448\)["amenity"="hospital"];%20\);%20/*added%20by%20auto%20repair*/%20\(._;\>;\);%20/*end%20of%20auto%20repair*/%20out%20body;%20\>;)

### Amenity

"amenity"="hospital" , For searching hospitals

I also discussed with my mentors my approach to scrap Hospitals Data & how I will store it on Github.

## Discussion

My entire discussion can be seen here

<https://forums.librehealth.io/t/project-develop-an-android-mobile-application-to-show-patient-friendly-costs-of-care/3685/14>
