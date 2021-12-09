<<<<<<< HEAD
# Group Project #2 - NFL Predicitons - Creating a Machine Learning Model to Predict NFL Matchups
#### UW Fintech - Fall 2021

---

## Description

This project uses Machine Learning and Neural Network techniques to predict the probibility of whether an NFL team will be victorius in there next weeks matchup.  By using stastistics from completed games in the season, this model transforms the data into a variety of features that is then able to put inputted into a predictive algorithm.  The algorithm output then shows the predicted probability that a team has to be victorious.  This predictive model is in the preliminary stages of development and by no means should be used for any sports betting activity.  

The sections of this notebook are as follows: 

* Import, Clean and Prepare the data for use in machine learning and/or neural network modeling. 
* [Insert Different Types of Models Used Here]]
* Analyze Results and Results Visualization

---

## Data Sources

The sources of data are as follows:

* [Sportsipy API](https://sportsreference.readthedocs.io/en/stable/) - API used to pull the most recent NFL games statistics. 

* [Sports-Reference.com](https://www.pro-football-reference.com/) - API used to pull the most recent NFL games statistics.

* [FiveThirtyEight - ELO Rating](https://github.com/fivethirtyeight/nfl-elo-game) - API used to pull the most recent NFL ELO statistics. 

* [NFL Team Stats 2002-2020 (Kaggle)](https://www.kaggle.com/cviaxmiwnptr/nfl-team-stats-20022019-espn?select=nfl_team_stats_2002-2020.csv) - NFL statistics for 2002 - 2020 NFL seasons. 

---

 ## Executive Summary

It has been three years since the Supreme Court legalized sports betting. Currently, only half of the states in the US allow sports betting, but still, the amount of money being bet on sports has quadrupled since becoming federally legal. 
Where there is opportunity for financial gain, there is often innovation. Due to the statistical nature of sports, machine learning methodologies seemed like a perfect fit for making sports game predictions. 

In this project we develop and compare multiple machine learning models and use them to make predictions on NFL matches.  The results of each model used ares disscussed in the following sections.

---

## Analysis and Conclusion Overview

Refer to the Jupyter Lab notebook for a more detailed view of the analysis, but a summary of the analysis and each machine learning techniuqe used can be seen in the following: 

### Neural Network

### Random Forest

### Logistic Regression 

### Conclusion  

---

## Technologies

This project leverages JupyterLab Version 3.0.14 in association with Anaconda distribution and the Conda package manager.  The following packages are also used: 

* [pandas](https://github.com/pandas-dev/pandas) - Data analysis toolkit for Python.

* [sklearn](https://scikit-learn.org/stable/) - Predictive data analysis.

* [keras](https://keras.io/) - Deep learning API running on top TensorFlow.

* [hvPlot](https://github.com/holoviz/hvplot) - A high-level plotting API for the PyData ecosystem built on HoloViews.

---

## Installation

Before running the application, install Python modules Pandas, hvPlot, SQLAlchemy and Voila:

```python

  conda install pandas

  conda install -c pyviz hvplot

  pip install -U scikit-learn

  pip install tensorflow

```
 
---

## Contributors

Jacob Vissering - [email]

Lisa Bailey - [email]

Niki van Dyck - [email]

Joshua Creveling - josh.creveling22@gmail.com

---

## License

MIT
=======
# NFL Predictions 
## Summary 
Where there is an opportunity for financial gain, there is often innovation. Due to the statistical nature of sports, machine learning methodologies seemed like a perfect fit for making sports game predictions. 

## Goal 
To develop and compare multiple machine learning models and to make predictions on NFL matches. 

## Scoping 
While scoping this project, we found lots of information on sports predictions.  After vetting a few data sources, we found the API from Sports-Refernace.com to be the most straightforward API to use.  We also completed a reasonableness validation and reviewed Sports-Refernace.com projection data vs. posted box scores.  IN addition to reviewing overall reasonableness, the team also spent a few hours reviewing the code by line to ensure we understood how the results were calculated.  

## Data Preparation
Using the API, we pulled all statistical data available for completed games and the schedule of future games. We then created a weekly prediction data frame to enable the ability to analyze both historical week accuracy and to predict the win/ loss in the coming weeks. All win/loss predictions were the results of the away team win (1) vs. a home team (0).     

## Machine Learning Models 
We applied the prepared week data set to the following models: Logistic Regression Scaled, Logistic Regression Unscaled, Random Forest, and  Neural Network/ Tensorflow.  Of the models tested, the Random Forest learning model reflected the highest predicted of game outcomes between the weeks of 2-13, at a prediction rate of 66.2%     

## Conclusion
Were we successful? 
* To win money on a bet with -110 odds, a winning percentage of 52.4% is needed.
* Our best model returned a winning percentage of 66.2%.

What about picking favored winning teams?
* Odds are lower
* To breakeven the required winning percentage goes up

Example: Denver Broncos vs. Detroit Lions (W14)
* Broncos -375
* Assuming you bet a sample of 100 bets on -375 favorites, you would need a prediction percentage of 79% to break even.

## Addendum / Supporting Details

![update_placeholder](https://github.com/link)
>>>>>>> 31b817fc11aaa0007b26ad2fa629e9ada7455b76
