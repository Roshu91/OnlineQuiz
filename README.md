Online Quiz System

An online quiz system built on PHP, JS, HTML, MySql.This web application was developed for non profit organisations to conduct online Exam for students of various educational institutions, Schools, Colleges, Universities etc.
This project is simple and easy to implement, updated by Roshan Pradhan (https://github.com/Roshu91).You are free to modify and re-distribute

Features: 

1. Timer support.
2. Admin control to "Enable" and "Disable" the quiz.
3. Registered users can start and finish the quiz at any time.
4. continue exam option if error occured. 
5.  Detailed analysis of the quiz results by both admin and registered users.

Implementation:

1. Create a new database in MySQL.
2. Run the SQL query in "quizzer.sql".
3. Open the file "dbConnection.php" and change the Server name, Username, Password and Database name.
3. Visit the home page in browser. Use the "Admin Login" link to login to Admin Panel. Default user - 'sonudoo' pass - '1234567890'

#How to Use

1. Use the Admin Panel to set up quiz. Quiz won't be enabled unless you click the "Enable" button. Click on the same to enable an added quiz.
2. Scores are updated realtime on the server, however the leaderboard will be updated only when the user finishes the quiz, or there is a time out or the admin ends the quiz by clicking on "Disable" button.
3. Once the admin clicks on the disable button, the quiz ends for all the users taking that quiz, irrespective of their active or inactive state (whether logged in or left the quiz in the middle only). The leaderboard will be updated either when a user "Finishes" his /her quiz and when the admin "disables" the quiz. 
4. Once the quiz is disabled, the quiz becomes inaccessible. If the quiz is enabled again later, only those user who have not already taken the quiz can take the quiz.
5. It is recommended that you Enable the quiz when all the users are ready and disable the quiz when all the users have completed the quiz or time limit of taking the quiz has exceeded.

#Bugs:

1. Too many SQL queries, needs optimization. Yet not suitable for more than 200 simultaneous user.
2. Security issues, need to sanitize the URL queries.
