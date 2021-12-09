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
