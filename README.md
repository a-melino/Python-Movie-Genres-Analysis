# Python & Pandas: Movie Genres Data Analysis Project

![Header](Images/header.png)

#
#### by Alex Melino
#

### Background Information

This is a sample project using the Pandas Python library to perform an analysis on a dataset of over ten thousand movies spanning from 1960 to 2015. The analysis is intended to focus on the genres of the movies and how the different genres have performed in terms of popularity, budget, revenue and profit over time.

The following libraries and dependencies are required to run this Jupyter Lab notebook: Pandas, Seaborn, Matplotlib. They can be installed using a basic '!pip install' command.

#
### Research Questions and Hypotheses

This project seeks to answer some questions and confirm or deny some hypotheses relating to movie genre patterns. The following is a list of questions and hypotheses that are explored:

Research Questions:
1. Which genres are the most common (number of movies made)?
2. Which genres have high avg. budget and revenue?
3. Which genres have high avg. profit?
4. Which genres have high avg. popularity?
5. Which genres have highest number of movies with a voting avg >= 8?


Research Hypotheses:
1. The best movies according to vote avg. return the highest profit and revenue.
2. The best movies according to popularity return the highest profit and revenue.
3. Highly budgeted movies return high profit.
4. Highly budgeted movies have high popularity.
5. Movies have made more profit over time (based on genre).


### Data Exploration and Cleaning

The dataset used comes from the IMDB website and it contains a lot of information that was unnecessary to the analysis being performed for this project. Therefore, some data cleaning steps were taken to set up the data for easy visualization. The dataset file can be found in the 'Resources' folder of this directory as 'imdb_movies.csv' while the python code can be found in the main directory as 'movie_genres_analysis.ipynb'.

The first steps here were to remove duplicate rows and remove rows with null values in the 'genres' column as that column would be crucial to the analysis.

Next, a new calculated column named 'profit' was created based on the 'revenue' and 'budget' columns.

The unneeded columns were then dropped, and a new dataframe was crated to work with the data. 

![Code1](Images/code1.png)

Finally, the 'genres' column was split and used as an index. That index was converted to a new column ad added to the working dataframe.

![Code2](Images/code2.png)
#

### Data Visualization

The following visualizations were created using Pandas, Matplotlib, and Seaborn libraries to answer the research questions and hypotheses listed above. Copies of the visualizations are saved .png files in the 'Images' folder of this repo.


#### Research Questions:

1. Which genres are the most common (number of movies made)?

A pie chart and a bar chart were used to visualize the proportion of all movies for each genre.
![Pie1](Images/pie1.png)
![Bar1](Images/bar1.png)

2. Which genres have high avg. budget and revenue?

A grouped bar chart to show the average budget and revenue based on each genre.
![Bar2](Images/bar2.png)

3. Which genres have high avg. profit?

A bar chart to display the genres with respect to their average profit.
![Bar3](Images/bar3.png)

4. Which genres have high avg. popularity?

A bar chart to display the genres with respect to their average popularity rating.
![Bar4](Images/bar4.png)

5. Which genres have highest number of movies with a voting avg >= 8?

A bar chart to display the movies per genres with a rating of 8 or higher.
![Bar5](Images/bar5.png)

#
#### Research Hypotheses:

1. The best movies according to vote avg. return the highest profit and revenue.

 Regression scatter plots to visualize the correlation between vote average, revenue and profit. Vote average appears to have a slightly positive correlation to both revenue and profit.
![scatter1](Images/scatter1.png)
![scatter2](Images/scatter2.png)

2. The best movies according to popularity return the highest profit and revenue.

 Regression scatter plots to visualize the correlation between popularity, revenue and profit. These plots show a strong positive correlation between a movie's popularity and high revenue and profit.
![scatter3](Images/scatter3.png)
![scatter4](Images/scatter4.png)

3. Highly budgeted movies return high profit.

A regression scatter plot to visualize the correlation between budget and profit. There is a medium strength positive correlation between a movie's budget and its profit.
![scatter5](Images/scatter5.png)

4. Highly budgeted movies have high popularity.

A regression scatter plot to visualize the correlation between popularity and budget. There is a medium strength positive correlation between a movie's popularity and its budget.
![scatter6](Images/scatter6.png)

5. Movies have made more profit over time (based on genre).

A heatmap to visualize how the average profit has behaved for each genre over time. Certain genres have shown a clear increase in profit over time, namely action, adventure, animation, family, fantasy, and sci-fi movie genres.
![heatmap1](Images/heatmap1.png)




#
### Further Analysis

Further analysis can be conducted on other aspects of this data as the focus of this project was on genres specifically. Trends with cast, production companies, release dates, etc. could all reveal valuable and useful trends.

Additionally, further visualization software and libraries could be used to create deeper and more innovative visualizations and analysis.

