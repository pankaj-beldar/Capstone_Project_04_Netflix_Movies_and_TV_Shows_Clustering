# Netflix_Movies_and_TV_Shows_Clustering

# <font color='green'>**Problem Statment**</font>


This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.

In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

# <font color='red'>**Milestones**</font>

1. Importing Libraries
2. Import Data
3. Data Overview
4. Data Cleaning
5. Data Visualization with EDA
6. Text Processing
7. Model Selection and Hyper Parameter Tunning
   
   **PART A: Modelling with Word2vec**
   
   **PART B: Modelling with CountVectorizer/tfidfVectorizer**
8. Recommendation System
9. Conclusion

# **Exploratory Data Analysis**


1. The attribute **'diector','cast','country','date_added','rating' consists of missing values.** To tackle with missing values , we will replace 'country' and 'rating' missing values by most frequent entity that is 'United States' and 'TV-MA' respectively. missing values in 'cast' by 'unknown'. There are around **30.68 % values are missing in 'director'**, hence we decide to drop it.


2. **69% of the content available on Netflix are movies; the remaining 31% are TV Shows** .**Netflix has 5377 movies**, which is more than double the quantity of TV shows. In recents year more number of TV Shows are released as compared to Movies on Netflix. Less number of TV shows and Movies were released in 2020-2021 due to corona virus pendamic. **Most of the Movies/TV Shows were added in the month of December and January.**


3. **Number of Movies added on Netflix are more as compared to TV Shows throughout the year. In recent few year more number of TV Shows were added on NetFlix as comapared to Movies , We can say Netflix is more focusing on TV Shows than Movies.** 


4. **United States, India, United Kingdom, Japan, South Korea, Canada, Spain, France,Egypt and Turkey are the Top 10 countries** which produces most of the content on Netflix. United States produced most of the content on Netflix also number of movies releasd are more than TV Shows in United States. In India, Canada, Spain, France, Egypt and Turkey , Most of the content on Netflix is Movies. United Kingdom has almost equal production of Movies and TV Shows. In Japan and South Korea, Number of TV Shows are available on Netflix on large scale. 

5. It is observed that, in each category, Quantity of Movies is more than the Quantity of TV Shows.**The Availabilty of the Adult Content is more on Netflix and Least for the Kids**.


6. Popular Movies ratings are **TV-MA, TV-14, R, TV-PG, PG-14 and PG**. It is observed that Adults and Teens are mostly active on Netflix. Popular TV Shows ratings are **TV-MA, TV-14, R, TV-PG, PG-14 and PG**.


7. **Top 5 Genres in 'TV Shows' are Kid's TV, TV Dramas ,TV Crime Shows, TV Comedies, TV Romantic.** **Top 5 Genres in 'Movies' are Documetaries, Stand up Comedy, Drammas and International Movies, Comedies and Independent Movies.**It is observed that **1608 TV Shows has only one season**. The count of longest running TV Shows is very less. 

8. Famous Actors on Netflix based ont the Frequency of their occurance on screen are Anupam Kher, Takahiro Sakurai Shah Rukh Khan, Om Puri and Boman Irani and so on. Most of the **Movies/TV Shows has duration around 100 min.**

9. United States is producing maximum International TV Shows, TV Dramas, Sci-fi and Fantacy TV shows, International Movies. **India, UK, Spain ,Egypt,Mexico and Turkey is having most of the Content as Dramas and International Movies.**


10. **It is observed that content available for kids is less as compared to other categories. Content available for Adults is more in almost every country expect India. In India, Most of the content is available for Teens. Netflix should foucus on Teen and Adult Contents to generate maximum revenue.** **Spain and Mexico is producing highest Adult Content on Netflix almost 84% and 77% respectively.**


# **Clustering with Word2vec**

1. K-Means with 0.6092 silhouette_score with word2vec has optimum number of clusters as 6

2. K-Means with Elbow method with word2vec has 5 optimum clusters.

3. Agglomerative Clustering with dendogram with word2vec has 5 optimum clusters

4. Agglomerative Clustering with 0.53 silhouette_score with word2vec gives 4 clusters

5. Affinity propagation clustering with woed2vec has 5 optimum clusters

# **Clstering with CountVectorizer**

1. It is observed that , after using CountVectorizer and tfidfVectorizer, we get the less silhouette_score as 0.032

2. Hence we can say word2vec word embending method is more suitable for our model.


