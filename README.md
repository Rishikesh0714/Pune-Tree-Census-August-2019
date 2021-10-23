# Pune-Tree-Census-August-2019

## Overview 
My main motive is to understand the Tree census or record of my hometown Pune city .I am proud to say that Pune city is smart city and I got this data from website .Note - Data is updated on August 2019. Wards are how here Pune city is divide under corporate officials

- [Pune Data-Store](http://opendata.punecorporation.org/Citizen/CitizenDatasets/Index) 
- [Data File](http://opendata.punecorporation.org/Citizen/CitizenDatasets/DownloadDataset/483?filepath=%2FDocuments%2F483%2FPune%20Tree%20Census%20August%202019.zip)

This data include many features like location of trees , size canopy , common names etc.
I will used this data to hopefully plot it on interactive map using Leaflet library

## Steps Involved

1. Step 1 :- Data Reading (only one file multiple files) with readr package I had large data that's why I choose just one file containing Number of Rows: 9623. 
2. Step 2 :- Data cleaning and preparing. There are 40lakhs plus rows and 28 features. I took only features I need for ploting.
3. Step 3 :- Making Data frame with chosen features make sure it contain Longitude and Latitude data.
4. Step 4 :- Dividing Data Ward wise . I have huge data which can strain the app to process so I decided to filter previous deploying .
5. Step 5 :- I used icon function from leaflet library to show diffrent condition of trees on the map
6. Step 6 :- Then I used clustering and popupmessage function to make clusters and add message to consumable form 
7. Step 7 :- In the last step I  deployed my app on Rstudio's Shiny server In the Navbar Layout format.

## Contents

- Data = Data Required 
- icons = Icon pic for different condition of plant (Healthy, Average, Death)
- index.html = I was trying to deploy this app on github pages but failed since github only support static pages
- Pune Tree Census August 2019(Leaflet Assignment) = RMD - Main App code (Just for one ward) and structure HTML - Output of Markdown file in html format
- Leaflet Assignment = RMD - It contain some codes to incorporate all 49 lakhs rows without compromising loading time in app


## Conclusion/Notes

1. Data is very large and I took only small subset of it for there was latency in rendering the leaflet. You can Find whole data from above source
2. It may take little time to load sorry for inconvenience
3. Code for ward 21 to 77 is in Rmd file in my github Repo
4. I Tried to use all data but its taking too much time to render and my R is crashing.
5. There is many more entries in files name p1, p2, p3 and p5 all 1000000 rows. This visualization is not able to render whole data .
6. Feel free to use Data From Source above.
7. Shiny app [Pune Tree Census]("https://rishikesh.shinyapps.io/Leaflet_Assignment/?_ga=2.99219033.637745020.1635002308-1361479577.1625326529")
8. My Github[Repo]("https://github.com/Rishikesh0714/Pune-Tree-Census-August-2019")
