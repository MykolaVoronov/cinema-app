# CINEMA APP

This project simulates cinema ticket shop using Hibernate and Spring. This application has several possibilities:
* User authentication and authorization
* Adding new movie, cinema hall, movie session
* Creating order
* Display all the above information

#### Endpoints
* POST: /register - all
* GET: /cinema-halls - user/admin
* POST: /cinema-halls - admin
* GET: /movies - user/admin
* POST: /movies - admin
* GET: /movie-sessions/available - user/admin
* POST: /movie-sessions - admin
* PUT: /movie-sessions/{id} - admin
* DELETE: /movie-sessions/{id} - admin
* GET: /orders - user
* POST: /orders/complete - user
* PUT: /shopping-carts/movie-sessions - user
* GET: /shopping-carts/by-user - user
* GET: /users/by-email - admin

#### Technologies
* Apache Tomcat
* Hibernate
* Hibernate Validator
* Spring Core
* Spring MVC
* Spring Security
* MySQL
* Maven

#### Setup
1. Install and configure MySQL & MySQL Workbench and create schema
2. Install and configure Tomcat 9.0.56
3. Link the database to the application:

    * *In the src/main/resources/db.properties, change the db.user, db.password, and db.url parameters to the ones you used when configuring MySQL. db.driver and hibernate.dialect change if you are using another DBMS.*

4. After that you can run the application and login using:
   * username `alice-admin@i.ua` with password `admin123` to login as admin
   * username `bob-user@i.ua` with password `user1234` to login as user