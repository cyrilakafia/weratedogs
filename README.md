# Wrangle and Analyze Data

## Gathering Data
The data was gathered from three different sources and in three different formats as described below:

1. The WeRateDogs Twitter archive. This file was provided by Udacity and was downloaded manually by clicking the following link: twitter_archive_enhanced.csv and was saved as a csv file.

2. The tweet image predictions. This file was hosted on Udacity's servers and was downloaded programmatically using the Requests library and the following URL: image_predictions.tsv and was saved as a tsv file.

3. Retweet and Favourite count for each tweet. This file was queried from Twitter's API using the Tweepy library and the tweet IDs in the WeRateDogs Twitter archive. The data was stored in a text file file.

## Assessing Data
The three pieces of data were assessed visually and programmaticlly for quality and tidiness issues.
* Visual Assessment: Each piece of gathered data is displayed in the Jupyter Notebook for visual assessment purposes. Once displayed, data was additionally assessed in an MS Excel.
* Programmatic Assessment: Pandas' functions and methods was used to assess the data.

### To meet specifications...
* Only original ratings (no retweets) that have images were kept. Though there are 5000+ tweets in the dataset, not all are dog ratings and some are retweets.
* The fact that the rating numerators are greater than the denominators does not need to be cleaned. This unique rating system is a big part of the popularity of WeRateDogs.

## Cleaning Data
All issues documented while assessing data was cleaned in the "Cleaning Data" section in the [wrangle_act.ipynb](https://github.com/cyrilakafia/wrangle-data/blob/main/wrangle_act.ipynb).
* Before cleaning, a copy of original data was made
8 During cleaning, the define-code-test framework was used and documented.
* The result was 2 high-quality and tidy master pandas DataFrames.

## Storing Data
In the "Storing Data" section in the [wrangle_act.ipynb](https://github.com/cyrilakafia/wrangle-data/blob/main/wrangle_act.ipynb) notebook, the cleaned master DataFrame is stored as a csv file with name `twitter_archive_master.csv`. The addidional file was stored as `twitter_archive_tweet_info`.

## Analyzing and Visualizing Data
Finally, visualizations were made on the cleaned data with `matplotlib` and `seaborn` after which the data was stored.

## Reporting
1. A written report called [wrangle_report.html](https://github.com/cyrilakafia/wrangle-data/blob/main/wrangle_report.html) was created to briefly describe the wrangling efforts. This was framed as an internal document.

2. A second report called [act_report.html](https://github.com/cyrilakafia/wrangle-data/blob/main/act_report.html) was created to communicate all the insights through visualizations produced from the wrangled data. This was framed as an external document (blog post).


## References

1. https://help.start.gg/en/articles/1987102-customizing-text-with-markdown#:~:text=Aligning%20Text,the%20text%20in%20div%20tags.

2. https://www.w3schools.com/PYTHON/matplotlib_pie_charts.asp

3. https://www.digitalocean.com/community/tutorials/pandas-merge-two-dataframe
