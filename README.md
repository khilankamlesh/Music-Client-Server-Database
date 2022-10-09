# Music Client-Server Database

## Prerequisites ##
This project was created in SQL using PostgreSQL, with the JDBC driver installed, and Java in Project SDK version 11.0.2 using IntelliJ IDEA Community Edition.

This was the third of three projects as part of the Full Stack Applicaiton Development module at the University of Birmingham, focusing on JDBC and Java Networks/Socket programming as well as SQL using postgreSQL.

## Goal ##
The goals of this project are to:
* Create and populate a music database
* Implement a basic multi-threaded server that continuously listens for connections and creates a new thread for each client connection
* Implement a basic client program that continuously reads the name of the artist from the console and prints the response from the server, until the user types ‘stop’

## Project Layout ##
* 'music_create.sql' contains SQL commands to be run in postgreSQL to create a music database
* 'music_data.sql' contains SQL commands to be run in postgreSQL to populate the music database
* 'ER-model.png' is a diagram showing the Entity-Relationship of the music database as seen [here](ER-model.png)
* Extract 'FSADAssign3_Khilan_Kamlesh_2307483.zip' and open folder as project in IntelliJ IDEA Community Edition 
  * 'Assignment3/src' contains classes to create the Server and Client Threads as well as take input from the user and perform SQL queries.

## Instructions ##
1. Open SQL Shell, connect to your default postgres database and run the files 'music_create.sql' and 'music_data.sql' with the \i command, followed by the file path.
2. Extract 'FSADAssign3_Khilan_Kamlesh_2307483.zip' and open folder 'Assignment3' as a project in IntelliJ IDEA Community Edition.
3. Open file 'Credentials.java' located in 'src' folder in IntelliJ. Edit the variables 'USERNAME' and 'PASSWORD' with your own postgres credentials.
4. Run 'Server.java' to start the server and then 'Client.java' to create a client. Multiple clients can be created by running 'Client.java' again.
