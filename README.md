#Personalized Restaurant Recommendation System

Imagine that you just land on a new city and you want to find the best restaurants around at your preference? This system is built for you :-) </br>

The frontend was done by HTML, CSS and Javascript. AJAX was used to communicate with the backend. </br>
The front end codes are in /WebContent</br>
</br>
The backend is composed of three java servlets that allows the user to explore, visit and get recommended restaurants. </br>
Java servlets codes are in /src/api </br>
For the backend, it connected to SQL dababase uisng JDBC. We used MySQL to store three tables: 1. user table 2. restaurant table 3. the visiting history. Table 1 and 3 are related by the user id, table 2 and 3 are related by the restaurant business id </br>
Database interface were in /src/db </br>
</br>
For the recommendation algoriths, we used item based collabarative filtering. The GPS location was first acquired and used to query the Yelp API to get the list of nearby restaurants and save them into the restaurent table. And the users visited restaurant was obtained and their categories were extracted into a list of categories. The recommended candidates were received by querying the visited categories from the restaurant table. Finall the visited restaurants were removed from the recommendations and sent back to the user.</br>
/src/model</br>
