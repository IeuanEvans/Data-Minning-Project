
#  Predicting Professional Road Cycling Race Results



Analysing statistics from historical sporting events can inform coaches and players to facilitate better decision making and subsequently better results in competition. Sports analytics can also be used to forecast winning athletes and team, which offers financial value to bookmakers and bettors.     

High quality data is essential for building ML model that performs well. Data was available for this project at procyclingstats.com a database driven website that stores cycling statistics, results, and rankings.   

* I am in still in the process of tidying and organsing the Ipython files for this project. Repo links in the table below will be working soon. 

|__Problem__|__Methods__|__Libs__|__Repo__|
|-|-|-|-|
|[Data Collecting](#scraping-data-from-procyclingstats.com-for-machine-learning)|Parsing web documents (`HTML` and `XML`) |`BeautifulSoup`, `lxml`|[Click](https://github.com/IeuanEvans/ProCycling_Project/blob/master/Web_Scraping_PCS.ipynb)|
|[Data Preprocessing](#processing-data-for-machine-learning-project)|Data cleaning, Data formatting, Data sampling|`Pandas`, `Numpy` |[Click]()|
|[Feature Engineering](#processing-data-for-machine-learning-project)|Aggregating features, feature normalisation|`Pandas`, `Numpy`, `Matplotlib`, `sklearn`|[Click]()|
|[Modeling](#training-model)|Model training, XGBoost, Data Splitting|`Pandas`, `Numpy`, `Matplotlib`, `sklearn`|[Click]()|
|[Hyperparameter Tuning](#tuning-xgboost-hyperparameters)|GridSearchCV XGBoost train_test_split|`Numpy`, `Pandas`, `sklearn`, `xgboost`|[Click]()|
|[Model Validation](#comparing-model-predictions-against-fan-predictions)|Sorting algorithms|`Numpy`, `Pandas`|[Click]()|



## Data Collection (Web Scraping)

As this was my first project of this kind I needed to find an effective way of extracting data off ProCyclingStats.com and storing it in a format ready for analysis. I highly rate Corey Schafer's YouTube channel for learning Python, fortunetly he has a video tuturial on webscraping with BeuatifulSoup and Requests libraries, which I used along with BeuatifulSoup library documentation by crummy.com.

I wrote a script that runs through thousands of race results and rider profile website pages and writes the relavent statistics (e.g. date, distance, average speed, top-10 wins etc.) to csv files.

<details>
  <summary>Click to expand!</summary>
  
  ![](images/Sraping_diagram.png)

</details>

## Data Preperation 

Data for some variables contain unwanted characters such as 'kg' for weight and 'm' for height. Some data is missing completly, if I recall correctly, the variables that were missing the most data were rider age and 'course profile' (race hilliness). For age, missing data were replaced with average height of all the riders. For course profile, missing data were replaced with course profile average for that race (i.e Paris Roubaix). 

Feature to be included in the furture: 
1) Rider form: has the rider improved from last season?
2) Weather: particular wind because air resistance plays a major role in the outcome of bike races.
3) Team mates: does the rider have support from team mates in the race and how strong/experienced are their team mates.
4) Home nation race: does racing in your home country offer any performance advantage

</details>

## Explore the Data



</details>


## Train the Model

Visualizations

</details>

## Evaluate the Model

Visualizations

</details>

## Make Prediction

The data includes ten seasons with the most recent data being for 2020. Since then, prestidgous bikes races have been ridden namley the 'spring classics'. This offers a good oppertunity to measure my model up against.

</details>
