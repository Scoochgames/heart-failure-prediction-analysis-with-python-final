# heart-failure-prediction-analysis-with-python-final
Analyzing a heart failure dataset with python for a final unit project at Mountainland Technical College

The dataset: https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction

## Data cleaning 
I checked the data for null-values by df.info() and I also dropped any rows that were complete duplictes of each other via df.drop_duplicates() (there were none).

After further investigation I have found outlires of 0 where it doesn't make sense to have 0's (Cholesterol and Resting BP).
Because of this I will be dropping the rows with 0's in incorrect places.
There was 172 rows with 0's that didn't make sense. 172 is a good chunk of the original 918 but dropping the entire rows is a method that is justifiable.

## Plots
All plots will be attached to the main project as ____.png under the folder 'plots'

I used aggregation to change the raw ST_Slope counts into percentages. The resulting bar plot immediately shows the percentage of people who received a heart disease diagnosis for each ST-Slope category, which gives a direct view of the risk.

For the second plot, I used a kdeplot (density plot) to see where most patients fall based on Maximum Heart Rate. Setting hue='HeartDisease' creates two separate curves on the same plot, and you can immediately tell that people with heart disease tend to have a lower peak heart rate compared to healthy people.

I used this code to make a scatter plot of patient Age against Cholesterol. The plot uses different colors and shapes to mark patients based on their Heart Disease status. The goal is to see if Age and Cholesterol levels alone cause the 'Heart Disease' and 'No Heart Disease' groups to visually separate or cluster.
