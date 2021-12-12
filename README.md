# NFL Predictions - Creating a Machine Learning Model to Predict NFL Matchups 
## Summary 
Where there is an opportunity for financial gain, there is often innovation. Due to the statistical nature of sports, machine learning methodologies seemed like a perfect fit for making sports game predictions. 

## Goal 
To develop and compare multiple machine learning models and to make predictions on NFL matches. 

## Scoping 
While scoping this project, we found lots of information on sports predictions.  After vetting a few data sources, we found the API from Sports-Reference.com to be the most straightforward API to use.  We also completed a reasonableness validation and reviewed Sports-Reference.com projection data vs. posted box scores.  IN addition to reviewing overall reasonableness, the team also spent a few hours reviewing the code by line to ensure we understood how the results were calculated.  

## Data Preparation
Using the API, we pulled all statistical data available for completed games and the schedule of future games. We then created a weekly prediction data frame to enable the ability to analyze both historical week accuracy and to predict the win/ loss in the coming weeks. All win/loss predictions were the results of the away team win (1) vs. a home team (0).

**Refer to Sportsipy_Create_Dataset_Notebook**

## Data Sources

* [Sportsipy API](https://sportsreference.readthedocs.io/en/stable/) - API used to pull the most recent NFL games statistics. 

* [Sports-Reference.com](https://www.pro-football-reference.com/) - API used to pull the most recent NFL games statistics.

* [How To Predict NFL Winners Guide](https://www.activestate.com/blog/how-to-predict-nfl-winners-with-python/) - Guide used to assist in using API

* [FiveThirtyEight - ELO Rating](https://github.com/fivethirtyeight/nfl-elo-game) - API used to pull the most recent NFL ELO statistics. 

* [NFL Team Stats 2002-2020 (Kaggle)](https://www.kaggle.com/cviaxmiwnptr/nfl-team-stats-20022019-espn?select=nfl_team_stats_2002-2020.csv) - NFL statistics for 2002 - 2020 NFL seasons. 

## Machine Learning Models 
We applied the prepared week data set to the following models: Logistic Regression Scaled, Logistic Regression Unscaled, Random Forest, and  Neural Network/ Tensorflow.  Of the models tested, the Random Forest learning model reflected the highest predicted of game outcomes between the weeks of 2-13, at a prediction rate of 66.2% 

**Refer to Model_Prediction_Workbook**

## Conclusion
Were we successful? Examples to consider:
* To win money on a bet with -110 odds, a winning percentage of 52.4% is needed.
* Our best model returned a winning percentage of 66.2%.

What about picking favored winning teams?
* Odds are lower
* To breakeven the required winning percentage goes up

Example: Denver Broncos vs. Detroit Lions (W14)
* Broncos -375
* Assuming you bet a sample of 100 bets on -375 favorites, you would need a prediction percentage of 79% to break even.

We believe our project was a success. We initially set out to create a model that could predict at least 60% of NFL games accurately. At that rate we thought there was a chance to make money. Our best model returnd an average accuracy throughout the season of 66% so we did succeed in hitting that mark. Furthermore, we have multiple base models that we can update, iterate through, and try to improve. 

However, our model does predict a lot of favored teams and when betting on favorites, the return on your wager is a lot less (than if it was an even match). Your losses hurt you more than your wins help you. Therefore, in order to make money while betting on favorites we would need a higher accuracy rate than 66%. We will need to do further analysis on our model to determine if it has an appropriate accuracy level when just considering betting on favorites.

Also, when we compared our predictions to Ceasars Sportsbook for week 8 of this season we actually out predicted them by one game. We plan to do further comparison against major sportsbooks to grade our models.

Our key next steps to improve our NFL prediction models are to:
* Add Rolling Window or Trending Features which will enable the model to spot mid-season up-trends and down-trends.
* Add more defense stat features to our model

Our key next steps to enhance our model usage are (in terms of using the model to make smart wagers):
* Find an API to bring in live bettings odds to add to our betting sheet dataframe.
* Use compare confidence intervals & betting odds to find "best bets"


## Technologies

This project leverages JupyterLab Version 3.0.14 in association with Anaconda distribution and the Conda package manager.  The following packages are also used: 

* [pandas](https://github.com/pandas-dev/pandas) - Data analysis toolkit for Python.

* [sklearn](https://scikit-learn.org/stable/) - Predictive data analysis.

* [keras](https://keras.io/) - Deep learning API running on top TensorFlow.

* [hvPlot](https://github.com/holoviz/hvplot) - A high-level plotting API for the PyData ecosystem built on HoloViews.

## Installation

Before running the application, install Python modules Pandas, hvPlot, sklearn, and tensorflow:

```python

  conda install pandas

  conda install -c pyviz hvplot

  pip install -U scikit-learn

  pip install tensorflow

```
## Addendum / Supporting Details
Tableau Reporting 
https://public.tableau.com/app/profile/lisa.bailey/viz/NFLPredictionModelAccuracy/NFLPredictionModelAccuracy

![averages](https://github.com/jake-viss/UW_Fintech_Project_2/blob/main/Resources/season_averages.PNG)  
![weekly_comp](https://github.com/jake-viss/UW_Fintech_Project_2/blob/main/Resources/weekly_comp.PNG) 
![feature](https://github.com/jake-viss/UW_Fintech_Project_2/blob/main/Resources/random_forest_feature.PNG)
![plot](https://github.com/jake-viss/UW_Fintech_Project_2/blob/main/Resources/testing_outcomes.PNG) 

## Contributors

Jacob Vissering - jake.vissering@gmail.com

Lisa Bailey - balllisaann@yahoo.com

Niki van Dyck - nikivandyck@gmail.com

Joshua Creveling - josh.creveling22@gmail.com
