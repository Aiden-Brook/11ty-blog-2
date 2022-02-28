---
title: Using APIs to Fetch Data from Wikipedia
description: This post is about learning how to get data from an api to display data from Wikipedia.
date: 2022-02-10
author: Aiden Brook
tags:
  - javascript
  - beginners
  - webdev
---

APIs (Application Programming Interfaces) and microservices are changing the way companies implement IT systems. Many large organizations such as Amazon, Netflix, Uber, and many more are using hundreds of microservices in their systems. These microservices call on APIs to fetch data for a specific function. In this post, I will be using an IP/location API to query Wikipedia articles about my location. More information about microservices can be found [here](https://www.divante.com/blog/10-companies-that-implemented-the-microservice-architecture-and-paved-the-way-for-others)

## Fetching Data from an API

To begin fetching data from an API, you have to call on the API to go out and get the data. Once the data has been retrieved you can store it's data as a variable. So in this example, I am storing my coordinates, city, and state (regionName) as data from the API which I will later use to find my location in google maps and find Wikipedia articles about.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/tgr6k6mqxlqueinx5uz4.png)


## Wikipedia Querying Using Another API

First, we need to import `'@lrnwebcomponents/wikipedia-query/wikipedia-query.js'` to be able to use this API. We also need to add its dependencies to the package.json file. After this is finished, we can call on the API to show us related articles to our current location. We can do this by entering the data that we stored as city and state so that the API can fetch an article about my location.This is done in the render function using HTML.


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/wgwpq3fv6o4007kmsoi9.png)


I used a hotspot from my phone so my location is not really where I was, but this is what it looks like when the web page is ran.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/f2eu9m57zsncys70kzzy.png)
