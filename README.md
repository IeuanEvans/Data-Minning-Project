Professional Cycling Outcome Prediction Project 
======================

#### This research project uses publicly available data from https://www.procyclingstats.com/ 

## Step One: Data Mining/Web Scraping

As this was my first project of this kind I needed to find an effective way of extracting data off ProCyclingStats.com and storing it in a format ready for analysis. I highly rate Corey Schafer's YouTube channel for learning Python, fortunetly he has a video tuturial on webscraping with BeuatifulSoup and Requests libraries, which I used along with BeuatifulSoup library documentation by crummy.com.

I wrote a script that runs through thousands race results and rider profile website pages and writes the relavent statistics (e.g. date, distance, average speed, top-10 wins etc.) to csv files.

<details>
  <summary>Click to expand!</summary>
  
  ![](images/Sraping_diagram.png)

</details>

## Step Two: Data Cleaning and Processing 

Data for some variables contain unwanted characters such as 'kg' for weight and 'm' for height. Some data is missing completly, if I recall correctly, the variables that were missing the most data were rider age and 'course profile' (race hilliness). For age, missing data were replaced with average height of all the riders. For course profile, missing data were replaced with course profile average for that race (i.e Paris Roubaix).       

</details>

## Step Three: Analysis

Visualizations

</details>

