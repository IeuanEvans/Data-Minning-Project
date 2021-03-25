

This research project uses publicly available data from https://www.procyclingstats.com/ and machine learning to predicted professional road cycling results.

Step One: Data Mining/Web Scraping

I needed a way of extracting data off ProCyclingStats.com and storing it in a format ready for analysis. Corey Schafer's YouTube channel has a tuturial on webscrape using BeuatifulSoup and Requests libraries, in addition to beuatifulsoup documentation on crummy.com.

The script goes through each race results and rider profile page and writes the relavent statistics to a pandas dataframes (e.g. date, distance, average speed, top-10 wins etc.).
See below 

 
Step Two: Data Cleaning and Processing 


missing data
columns to make sure your data is homogeneous and clean
how you can link everything together to achieve your original goal.
Concatinagte some list

Game stat data, team stat data, and datetime data are merge later into a feature file (.npz) for the ML algorithm (Lasso Logistic Regression) 


Step Three: Analysis



Step Four:
Visualizations



