# lenta--hackathon
Approach to solving the tape hackathon, 2nd place ( public + private leaderboard)

Input files:
  hist_data.csv - file with date for training
  test.csv - a file with a date for validating a solution at a hackathon
  
Notebooks:
eda.ipynb - exploratory analysis
user_class.ipynb - classification of users into 7 groups (the number of clusters is obtained by the elbow method)
class_rec.ipynb - recommendations for groups
local_validation_groups.ipynb - combination of personal and group recommendations
  
  Operating procedure:
1. Run data_split
2. Run user_class.ipynb, get a dataframe with the division of users into groups
3. Run class_rec.ipynb, get a dictionary with recommendations for groups
4. Run local_validation_groups.ipynb, get model prediction
