# Steam-Predictions
An attempt to predict user scores for Steam games, using existing review data.

Installation - This notebook uses the following Python libraries:
  numpy
  pandas
  matplotlib
  sklearn
  seaborn
  
This project uses only one file as its source:
  Steam.csv - Sourced from Kaggle at: https://www.kaggle.com/nikdavis/steam-store-games

CRISP-DM:
1.Business Understanding

Are certain developers better at making games than others?
	• The is a wide discrepancy of results by developer, with the best achieving 95% and the worst as low as 20%
	• These numbers are based from developers with a sufficient sample size (10 minimum)
Does price influence quality?
	• More than most variables, not significantly
Which are the best genres?
	• It seems specialist genres, like Web Design and Illustration are the highest rated
	• Whilst Accounting is the lowest rated
	• This shows, perhaps unsurprisingly, that educational games are at the extremes of the opinion scale

2. Data Understanding

Do we have many null values?
	• Fortunately, this data was already very clean from a NAN perspective
Is any data that might be useful missing?
	• We could include review sentiment analysis, but this would be complex beyond the scope of my investigation
	• Critic reviews might also be helpful as they often differ from the public reactions
How do the numeric variables correlate with one another?
	• Generally fairly low correlations

3. Prepare Data

Create dependent variable
Deal with concatenated string variables
Create dummy variables for categorical variables

4. Model Data

A Linear regression built using almost the entire dataset

5. Results

Disappointing results with a low RSquared, however this was not entirely unexpected given the subjective nature of gaming.

6. Deploy

Results have been presented via Medium blog here: https://medium.com/@benkvodafone/can-user-reviews-help-us-decide-which-game-to-play-216a046ecb00

Note to Reviewer: I am very aware that my Python is in serious need of improvement, but as I do not use it in my day job, finding the time to fit best practises is extremely difficult.