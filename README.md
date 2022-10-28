# Analyzing-OTT-Platforms

Click here for the Video Walkthrough: [![Video Walkthrough](https://img.shields.io/badge/-Analyzing%20OTT%20Platforms-red??style=social&logo=Youtube&link=https://www.youtube.com/watch?v=XDs-nJZxyO4/view?usp=sharing)](https://www.youtube.com/watch?v=XDs-nJZxyO4/view?usp=sharing)

Notebook best viewed in Google Collab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ruchita1003/Analyzing-OTT-Platforms/blob/main/Analyzing_OTT_Platforms.ipynb)<br>

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
