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

The first chart I made is a scatter plot, which most the time does not require any data aggregation or sorting.
It was a comparison between age and cholesterol levels. The r-value is 0.05875823535807384, this is a very weak positive correlation.
