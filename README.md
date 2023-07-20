# MyKare_Health_Assignment

<img align="left" alt="Coding" width="153" src="Image/logo.jpg">

Built a User Management Application, where a user can register himself either as an ADMIN or as a USER. This application uses Role-based authorization.



___________________________________________________________________________________________________________________________________________________________

# Tech Stacks: 

* Java
* Spring Boot
* Maven
* MySql
* SpringData Jpa
* Hibernate
* Spring Security(Basic auth)
* Devtools
* Lombok

# Features :

* User registration
* User and Admin authentication
* Role-based authorization

# Admin Features:

* Can get all users.
* Can get a particular user based on email id.
* Can access the details of different users.
* Can delete a user based on email id.

# User Features:

* Register with the application and sign in.
* Can get a particular user by email id;



# Installation & Run

Before running the API server, you should update the database config inside the application.properties file.

Update the port number, username and password as per your local database config. server.port=8886

spring.datasource.url=jdbc:mysql://localhost:3306/mykaredb 
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.username=mysql username 
spring.datasource.password=YourPassword 
spring.jpa.hibernate.ddl-auto=update

# Endpoints
API Root Endpoint - https://localhost:8800/


* To register user: https://localhost:8000/user/register  (Can be accessed by all)
* To get all users: https://localhost:8000/user/all  (Can be accessed by ADMIN only)
* To get a particular user: https://localhost:8000/user/{email} (Can be accessed by all)
* To delete a user: https://localhost:8000/user/{email} (Can be accessed by ADMIN only)
