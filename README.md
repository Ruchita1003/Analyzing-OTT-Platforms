# Analyzing-OTT-Platforms

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
We shall add 3 more binary columns denoting which platform the movie/tv show is aired on.<br>
##### The master dataset will now compose of a total of 19,925 rows and 14 columns. (The number of rows might decrease depending on the result of the concatenation of the OTT platform datasets and IMDb dataset).

Click here for the Video Walkthrough: [![Video Walkthrough](https://img.shields.io/badge/-Analyzing%20OTT%20Platforms-red??style=social&logo=Youtube&link=https://www.youtube.com/watch?v=XDs-nJZxyO4/view?usp=sharing)](https://www.youtube.com/watch?v=XDs-nJZxyO4/view?usp=sharing)

Notebook best viewed in Google Collab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Ruchita1003/Analyzing-OTT-Platforms/blob/main/Analyzing_OTT_Platforms.ipynb)
