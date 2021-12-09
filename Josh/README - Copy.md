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
