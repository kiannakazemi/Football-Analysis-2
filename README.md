# Football-Analysis-2
Football Analysis using generators 

Consider the match data of the football world championships from 1872 to 2020 available for free on the Kaggle website:
https://www.kaggle.com/martj42/international-football-results-from-1872-to-2017

In this project I used itertools generators and libraries to build a pipeline that performs the following sequence of transformations and filters:

    - Use a generator to read the data
    
    - Convert each record into a dictionary by using column names as attribute names and then merge all dictionaries into one list.
    Es. The line on the 2020-12-09 US-El Salvador match must be converted to:
      {'date': '2020-12-09',
      'home_team': 'United States',
      'away_team': 'El Salvador',
      'home_score': '6',
      'away_score': '0',
      'tournament': 'Friendly',
      'city': 'Fort Lauderdale', 'country': 'United States', 'neutral':
      'FALSE'}
      
    - Process the dictionaries obtained in the previous step to calculate using the itertool libraries (and thus optimizing the use of memory) the total sum of goals scored by  Poland in all World Cup matches.
