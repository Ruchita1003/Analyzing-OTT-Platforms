# Analyzing-OTT-Platforms

Click here for the Video Walkthrough: [![Video Walkthrough](https://img.shields.io/badge/-Analyzing%20OTT%20Platforms-red??style=social&logo=Youtube&link=https://www.youtube.com/watch?v=XDs-nJZxyO4/view?usp=sharing)](https://www.youtube.com/watch?v=XDs-nJZxyO4/view?usp=sharing)

Notebook best viewed in Google Collab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ruchita1003/Analyzing-OTT-Platforms/blob/main/Analyzing_OTT_Platforms.ipynb)<br>

### Steps to run the project:
- Open the notebook in colab.
- Add the 4 CSVs to the data folder inside the colab.
- Select 'Run All' to run the entire notebook at once.

### How the data was gathered:
Our dataset is not readily available as a single CSV and we plan on putting it together in the following manner:

1)	We plan on concatenating 3 datasets from Kaggle in order to form an extensive one stop shop dataset that contains information regarding movies and tv shows available on Netflix, Amazon Prime Video and Disney+.<br>
•	Netflix Data - [Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
This dataset has one table in a CSV format containing 8807 rows and 12 columns.<br>
•	Amazon Prime Data - [Amazon Prime Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/amazon-prime-movies-and-tv-shows)
This dataset has one table in a CSV format containing 9668 rows and 12 columns.<br>
•	Disney+ Data -  [Disney+ Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/disney-movies-and-tv-shows)
This dataset has one table in a CSV format with 1450 rows and 12 columns.
The above mentioned 3 datasets seem to have null values and shall require handling based on the datatype and significance of the columns. Additionally, all 3 CSVs share the same 12 columns in common making it comparison on certain parameters more feasible.

2)	From IMDB data - [IMDB Dataset](https://datasets.imdbws.com) we also wish to append more columns such as “IMDb” ratings and “Genre” to the above concatenated dataset in order to facilitate more value propositions. These will be taken from the IMDb Dataset on Kaggle. We do not intend to use the entire dataset, rather just a tiny part of it. This dataset has multiple tables and the information required for this project shall be extracted from the “ImdbTitleBasics.csv” and “ImdbTitleRating.csv" files.<br>
We shall add 3 more binary columns denoting which platform the movie/tv show is aired on.<br><br>
### The master dataset will now compose of a total of 19,925 rows and 14 columns. (The number of rows might decrease depending on the result of the concatenation of the OTT platform datasets and IMDb dataset).<br><br>

### Value Propositions this project offers:

### <font color = 'blue'>***As a user which OTT platform should I subscribe to in order to gain maximum benfits in terms of the content and to avoid investments in multiple streaming platforms?***</font><br>
![image](https://user-images.githubusercontent.com/60042693/198736401-bbd8679b-2916-4c3d-8103-e56d9e1d69b5.png)<br>
#### <font color = 'green'>The stacked bar graph shows the distribution of movies or TV shows based on their genre within the 3 OTT platforms. It is very evident that content wise, Netflix has the most number of movies / TV shows, followed by Amazon Prime and then Disney+. <br> As one would expect, Drama, Comedy and Action are the genres with the most available content.<br> A very surprising aspect of this graph is in the genre Animation. One would expect Disney+ to have the most content in Animation as Disney+ caters to a younger audience. However, Netflix has more Animation content than Disney+. <br> In contrast to this, Dinesy+ has more Family content than the other 2 platforms as one would expect. <br>So, from a subscriber point of view, Netflix would be the best option as it has more content within most genres in comparison to the other 2 OTT platforms. </font><br><br>

### <font color = 'blue'>***Which platform offers the best Animation content?***</font>
![image](https://user-images.githubusercontent.com/60042693/198737106-befeab27-6bd2-4087-b13d-407cb753597c.png)
#### <font color = 'green'>In the above chart we can observe that animated movies have been highly ranked on all the three platforms. This could denote viewers high interest in this type of content. <br> One would expect Disney+ to dominate this aspect of content, but surprisingly it is Netflix that offers the most animated content.<br><br> **Bonus value proposition:** Amazon Prime lacks in this genre and should consider onboarding more of it in order to garner a diverse content and viewership pool. </font>

### <font color = 'blue'>***Given the short attention span of kids do animated movie ratings get affected by their duration?***</font>
![image](https://user-images.githubusercontent.com/60042693/198737286-a64fc64a-5cae-4175-a54e-8ce9baaffa80.png)
#### <font color = 'green'> Based on the scatter plot we can see that most animated movies are rated well. However, movies which have a duration under 20 minutes have performed extremely well. All such short movies are found in Disney+. So for children with a very less attention span, Disney+ would be a great option to keep them engaged. </font>

### <font color = 'blue'>***On which platform should  a production house release Halloween content (Horror movies/ shows) ?***</font>
![image](https://user-images.githubusercontent.com/60042693/198737379-2f2db85f-d110-48fd-8159-6816ce350fda.png)
#### <font color = 'green'>It is surprising to see that Disney+ has the highest average ratings in Horror movies/ TV shows, despite being a platform that caters to kids. However, while counting the total numbe of Horror movies/ shows on each platform we see that Disney+ has only 1 horror movie/ show and it is rated very high. <br> Netflix has the next highest average ratings for Horror with the sceond highest number of movies/ shows in that genre. Hence, Netflix would be a better platform to release a Horror film. <br><br>**Bonus value proposition:** Since, the one Horror movie on Disney+ has a high rating, they could consider adding more horror movies to diversify their overall content.

### <font color = 'blue'>***What are the top genres of each platform? How can they increase the variety content to attract target audience? ?***</font>
 ![image](https://user-images.githubusercontent.com/60042693/198737528-89e0042c-6c0b-4cc7-a37e-f53ddba11fbd.png)
#### **Wait what?! Where are the widely watched genres? Are they not the top rated? Lets take a look at the count of the least produced content on these three platforms**
![image](https://user-images.githubusercontent.com/60042693/198737565-5fef765e-7e03-45d2-b096-6a1dcb2ecd5d.png)
#### <font color = 'green'> While analyzing the top 5 genres in each platform, none of the above mentioned expected genres appear. A shocking discovery is that "News" is one of the highest rated genres in all 3 platforms. However, it has one of these least content genre-wise in all 3 platforms. Since, viewers enjoy watching news, by increasing the new related content in all platforms, the OTT platforms and viewers could benefit from it.</br><br>**Bonus value proposition:** If Netflix (which already has the most News content currently) decides to onboard more news content, it can capture interested viewers and can have dominance in this sphere!

  ### <font color = 'blue'>***Does the length of a TV show really affect its rating? Does the genre of a long running tv show matter?***</font>
![image](https://user-images.githubusercontent.com/60042693/198737722-f1dadff7-3cf9-4a5a-a076-7f13a310f370.png)
#### <font color = 'green'> The above graph explains how the average rating of a tv show is affected by it number of seasons. We expected the rating to decrease with the increase in number of seasons due to user disengagement, but the results of the above chart are surprising. There does not seem to be a inversely proportional relationship between number of seasons and average ratings.<br> We expected most of the TV shows with 1 season to do well, but that is not the case. The average rating of TV Shows with 1 season only is highly varied and has a ratings spectrum from 2.5 to 10. <br> Another interesting observation is that most of the TV shows with more than 5 seasons are highly rated if they are of "Comedy", "Reality-TV", "Talk-Show" genre, and the poorly rated ones are of "Action" and "Thriller" genre.<br> This could imply that viewers prefer long running TV shows which are laid back and easy to watch type. They lose interest if a long running TV show is of Action or Thriller genre.
 
 **Lets zoom in on two data points from the above graph and make a direct comparison of the ratings per episode for the following two shows:<br> 1) The Muppet Show (Average Rating: 8.4, Total Season: 5)<br> 2) PJ Masks (Average Rating: 5.4, Total Seasons: 5)**
 ### <font color = 'blue'>***Why does "The Muppet Show" have higher ratings than "PJ Masks" despite both being 5 seasons long?***</font>
 ![image](https://user-images.githubusercontent.com/60042693/198737956-f6169596-50c5-49ae-9784-fe1292ddef44.png)
#### <font color = 'green'> The Muppet Show (of the genre "Comedy" and "Family") seems to have a pretty consistent rating mostly between 7 and 8.5 through out the entire run of the show. We do not see any major upticks or downfalls. This can be reflective of its close to consistent performance. This can be attributed to the fact that Comedy tv shows usually do not have major plots in their story line which can make viewers upset or lose interest immediately<br><br>
 #### **Lets compare this with PJ Masks(of the genre "Action", "Animation")**
 ![image](https://user-images.githubusercontent.com/60042693/198737999-6cc7546b-4900-46f7-b3f0-ea62e265a4f2.png)
#### <font color = 'green'>It looks like PJ Masks had a bumpier ride than The Muppet Show. From season 1 to season 3 with medicore rating in the range of 6-7.<br>There was a huge dip in the ending of season 2 and begining of season 3 when the rating fell from 7.6 to 4.9.<br>And then there was a sudden uptick in season 3 episode 6 (5.7 to 7.5 ratings)<br><br>
#### **Stepping out of the dataset!!**<br>The sudden downfall in the ratings got us extremely curious, so we actually looked into what the end of season 2 and start of season 3 was about. We noticed that these episodes in question had a common theme. They revolved around "Halloween", "Wolfs". The show also often seems to have usage of foul language.  It could be possible that this theme caused kids to disengage.<br>We also dug into the reviews of the show on a website (https://www.commonsensemedia.org/tv-reviews/pj-masks/user-reviews/adult), and read similar opinions!</font><br><br>
#### **We now have a better intuition about why The Muppet Show has higher ratings than PJ Masks!!**
