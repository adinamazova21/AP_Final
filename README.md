# AP_Final
Link
YouTube video:
https://youtu.be/CkffSMYp4DM


Idea proposal
•	Problem or idea description
The idea of the project is to create a film recommendation system. Also, user should see general ratings.

•	Background information on the problem or idea
For data, which is one of the most important parts of machine learning systems, library that contains movie with ratings dataset is needed. For movie recommendation for user, content-based filtering will be implemented. This type of filtering provides movie filtration based on one user’s film choices. 

•	Available solutions with links

Netflix - https://www.netflix.com

YouTube - https://www.youtube.com

Ivi - https://www.ivi.ru

•	How to get the data?
There 	TMDB 5000 Movie Dataset on Kaggle datasets, which will be helpful for getting the data for movie recommendation system.


•	Brief description of the solution
For movie recommendation system:
1.	Movie dataset;
2.	General ratings of movies;
3.	Content-based filtering are needed. 
During completion of the project, the solution will have greater clarity.

•	Tech stack that will be used:
1.	Python as programming language;
2.	Jupyter Notebook for interactive computational environment and others.


Work process
For this project TMDB 5000 Movie Dataset on Kaggle dataset was implemented. It consists of 2 datasets: credits and movies.
Credits dataset consists of 4803 rows and 4 columns (Figure 1) and no zero values (Figure 2).
 <img width="356" alt="image" src="https://user-images.githubusercontent.com/125748426/219877971-64fd6050-9bdc-4f31-a232-e7d9c6311273.png">

Figure 1

<img width="352" alt="image" src="https://user-images.githubusercontent.com/125748426/219877992-462533c7-870b-4161-825a-d9b610a0e5e2.png"> 

Figure 2

Movies dataset consists of 4803 rows and 20 columns (Figure 3) and some null values (Figure 4).
 <img width="317" alt="image" src="https://user-images.githubusercontent.com/125748426/219878008-cc7cc30b-0cae-4653-8277-6f2cb94a3259.png">

Figure 3

 <img width="333" alt="image" src="https://user-images.githubusercontent.com/125748426/219878017-573317e7-0792-492f-9d35-b7dec4c59dba.png">
<img width="331" alt="image" src="https://user-images.githubusercontent.com/125748426/219878026-e734af2f-0e06-4c8f-bbbe-cfa04cf7bf7f.png">

Figure 4

Credits and movies datasets were merged by their ids (Figure 5).
 <img width="356" alt="image" src="https://user-images.githubusercontent.com/125748426/219878040-5248004d-7454-44d2-aafa-446a8abc6ace.png">

Figure 5

After that weighted scores of movies were calculated (Figure 6) and demonstrated in the table (Figure 7). 
 <img width="347" alt="image" src="https://user-images.githubusercontent.com/125748426/219878057-c94e6ccb-389d-4a44-8b76-1b9b58ae082e.png">

Figure 6

 <img width="351" alt="image" src="https://user-images.githubusercontent.com/125748426/219878066-62bf09b1-ecc9-4b19-8a20-132451736e6f.png">

Figure 7

Then, table of TOP 15 movies with highest weighted scores (Figure 8), bar charts of TOP 15 popular movies (Figure 9) and TOP 15 movies with high budget (Figure 10) were demonstrated. 
 <img width="278" alt="image" src="https://user-images.githubusercontent.com/125748426/219878070-45f14c2e-5786-488a-815e-129be1e894a9.png">

Figure 8

 <img width="387" alt="image" src="https://user-images.githubusercontent.com/125748426/219878076-80d16644-8619-47e8-beba-7430417a74f8.png">

Figure 9

 <img width="387" alt="image" src="https://user-images.githubusercontent.com/125748426/219878096-1c39d95d-c226-4413-b74f-27af92f906c5.png">

Figure 10

Next was finding movies with similar overviews by implementing steps of:
1.	Eliminating meaningless words such as an, that and etc,
2.	Replacing Nan values by empty space,
3.	Fitting and transforming data 
4.	Cosine similarity matrix creation and others (Figure 11).
 <img width="295" alt="image" src="https://user-images.githubusercontent.com/125748426/219878103-2c6f14e4-2e53-4a30-8743-45b965cf0b21.png">

Figure 11

Therefore, search was expanded to similar genres, keywords, cast and director name, if it was known (Figure 12).
 <img width="331" alt="image" src="https://user-images.githubusercontent.com/125748426/219878107-c895d952-57cf-421a-98fa-b16e605cdea0.png">

Figure 12

After that, collecting data and values, putting them in vectorizer, calculating cosine similarity, resetting index of movies dataset and performing reverse mapping were introduced (Figure 13).
 <img width="319" alt="image" src="https://user-images.githubusercontent.com/125748426/219878120-ef8f7626-7337-465b-b5ff-6157a0ab564d.png">
 <img width="313" alt="image" src="https://user-images.githubusercontent.com/125748426/219878125-2d1ecb9a-ad09-4c40-8068-5fffae2f4da6.png">

Figure 13

Finally, we got 15 movie recommendations by the movie we chose, based on different features such as overview, genre, cast, keywords and director (Figure 14).
 <img width="347" alt="image" src="https://user-images.githubusercontent.com/125748426/219878134-1952b2fd-e345-427b-8d67-ecd202b86ee2.png">

Figure 14


Conclusion 
Final project on movie recommendation system was made for the Advanced Programming course. For this, knowledge and skills acquired from lectures, practice sessions and self-education was used. As a result, skills, including coding in Python programming language, precepting and understanding machine learning and deep learning and so on, have been acquired and deepened.


Literature review
1.	https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata
2.	https://www.kaggle.com/code/ibtesama/getting-started-with-a-movie-recommendation-system/notebook
3.	https://youtube.com/watch?v=ijtxuF_5kEU&si=EnSIkaIECMiOmarE
