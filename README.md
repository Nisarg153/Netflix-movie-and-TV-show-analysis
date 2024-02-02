# Netflix analysis
Here I have used [Pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), [Plotly](https://plotly.com/), and [WordCloud](https://pypi.org/project/wordcloud/) for EDA purpose.

Using [Pandas](https://pandas.pydata.org/) I cleaned the data and did the following steps
  - First I checked how many NaN values I had
  - To check the NaN values I created matrix using missingno Library and check it in visualized form
  - Dropped Directores and cast columns from the dataset as those columns are not that much of use.
  - Removed the NaN rows from date_added column
  - changed data type of date columns from object to datetime
  - Added Year and month columns and changed their data type to integer as we will use that to analyze and visualize the dataset
  - Made categories of Adults, Teens, Older kids, and kids instead of rating to make analysis easier
  - We want to use country columns from analysis purpose so we replaced NaN to Unknown

For EDA purpose we used [Plotly](https://plotly.com/) to make visualization more interactive. (we can also use [Matplotlib](https://matplotlib.org/) but I used [Plotly](https://plotly.com/))
  - Using [histogram](https://plotly.com/python/histograms/), I analyzed
      - How many total Number of Movies and TV shows were released
      - How many Movies and TV shows were released based on age groups
      - How many Movies and TV shows were released from 2016 to 2022
      - Movie duration analysis
  - Top 10 Countries with the use of [barplot](https://plotly.com/python/bar-charts/)
  - Propotion of Movies and TV Shows and with that the propotion of every age groups in Movies and TV shows as well using [sunburst](https://plotly.com/python/sunburst-charts/)
  - [Treemap](https://plotly.com/python/treemaps) of Year, type, and age groups
  - [World Map](https://plotly.com/python/choropleth-maps/) to show the released movies and TV shows based on their geographic locaions
  - [Box plot](https://plotly.com/python/box-plots/) to identify the outliers, median, and mode and where the majority of the data lie
  - [Wordcloud](https://plotly.com/matlab/wordcloud/) of Movies and TV shows

# Conclusion
  1. There are 70% movies in the whole dataset.
  2. For kids there are only 5% of movies and 10 % tv shows.
  3. From 2016 to 2022 mostly adult movies and TV shows were released.
  4. Each year almost (1/3)rd of the teens movies and TV shows were released.
  5. From 2016 to 2022 TV shows were increaseingly being released.
  6. In USA total 3100 movies and TV shows were released.
  7. More than 800 locations are Unknown.
  8. Most of the movies are 90 - 110 min long.
