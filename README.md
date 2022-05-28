# Customer-Relationship-Management-by-Vimlesh
Author- Vimlesh Kr. Singh



Customer Relationship Management  

Name : Vimlesh Kumar Singh 
Reg No: 11905337
College: Lovely Professional University, Jalandhar, Punjab

Project Description 
Developing a web application with help of Spring, Hibernate, and HTML/CSS. The journey is about how to create a backend web application. The Customer Relationship Manager will keep track of all the customers. Adding new customers, editing their information, and deleting them when needed. 

Project Language(s) 
Java 
Prerequisite(s) 
Java, HTML, CSS 
Skills to be learned 
Spring Framework, Spring Core, Spring MVC, Hibernate, JDBC, ORM framework, Maven, JSP, HTTP, MySQL 
Overview 
Objective 
Customer Relationship Manager web application is widely used by managers to store, retrieve and modify their customers' information. This project is the implementation of a

backend web application where we can create, read, update and delete (CRUD) customer information. This exciting CRUD application will be built using Spring MVC, Hibernate (ORM framework), and MySQL (for managing RDBMS). 
Project Context 
Customer Relationship Management web application is used by the managers to store, retrieve and modify their customer information. 
Spring is one of the best frameworks for backend development while working on Java since it uses the MVC design pattern. For the front-end side, HTML and CSS have been used here. The purpose of the Spring framework is to allow designers and developers to focus on building a unique feature for their web-based projects rather than re-inventing the wheel by using the very basics of Java. You will be learning the Spring framework over the course of building this Customer Relationship web application. 
After completion of the project, you will learn how to use CRUD operations, MVC design pattern, and Object-relational mapping framework (by connecting the backend web app to a database) majorly. You will also be familiarized with HTML, CSS languages by then. 
Some of the advantages of web applications include: 
- Accessible from any Internet-enabled computer. 
- Usable with different operating systems and browser applications. 
- Easier to roll out program updates since only software on the server needs to be updated. - Centralized storage on the server means fewer security concerns about local storage. You can also use Spring Boot as it needs minimum configurations without the need for an entire Spring configuration setup. There are other frameworks as well like Node JS, Angular JS, etc. Finally, which technology to choose totally depends on what applications we want to build and also on developer requirements. If you're going to develop an app that depends on I/O, then go to Node.js. But if you want to build a super-fast application (eCommerce platforms, IoT, etc.) with a crazy amount of computing, then go to the Spring boot framework. 
The main context of this project is to learn to build a web-based CRUD application using Spring MVC. 
Get started with the following links to refresh your memory (and maybe learn something new too ;) ) - 
Starter Resources 
- MVC Framework 
- Spring Framework 
- Hibernate

- Basics of CRUD 
- JDBC vs Hibernate 
Product Architecture 


The product Architecture can be divided into 4 stages as follows: 
1. Design the front-end of the web app using HTML and CSS. 
2. Implement controllers to handle requests and responses for all the CRUD operations. 3. Implement the hibernate queries to fetch results 
4. Integrate the web app with the database to fetch data from the backend The flowchart is as follows: 
High-Level Approach 
1. Create a Maven project using spring MVC. 
2. Design the database table for customers. It should have a unique id, first name, last name and an email id. 
3. Once the database table design is ready, write the controller, service and dao layers to execute the CRUD operations. 
4. Build the front end of the web app using HTML, CSS to accept input and render data correspondingly. 
5. Integrate the controller with the database to successfully build the Customer Relationship Manager web application.


Primary goals 
1. Every user should have the following privilege operations- 
● Create a customer 
● Read the customer details 
● Update customer details 
● Delete a customer 
2. While deleting a customer, all the associated information should be deleted from the database. 
Task 1 
Setting up the development environment 
First off you need to set up the development environment for the web application project. For a java web development project, you need to install Java and Maven. Additionally, you need a code editor or IDE to write the code, configure a database to store the data, and finally configure a local server to host the application. 
Requirements 
1. Install MySQL workbench or SQL Developer in your local system as we will be using MySQL/Oracle as our database 
2. Install Java (JDK 1.8) 
3. Install Maven 3 or higher 
4. Install IntelliJ (Community edition) or Eclipse 
5. Install Tomcat 6 or higher to run the web application locally 
6. Do the environment setup for Java and Maven on your local machine 7. Feel free to change the server running PORT if needed 
Check the versions of java and maven to know whether you have successfully installed them or not 
java -version




mvn -v



Congratulations!!! Your initial set up is done! 
References 
• Installing mysql workbench on Windows 
• Installing Oracle on Windows 
• Installing Java 
• Installing Maven 
• Installing Eclipse 
• Installing IntelliJ IDEA 
• Installing Apache TOMCAT 
Expected Outcome 
You should be able to set up the initial development environment. 
 2 
Creating a new Spring MVC project and a new table in the database 
After the initial setup is done, you need to add a new Maven project in the IDE installed and also need to add a new table in the database to store and retrieve data. 
Requirements 
1. Create a maven project using the Spring MVC archetype. You can refer to the below reference to set up your first maven project using the spring archetype to pom xml step-wise. 
○ Creating a maven project using in IntelliJ IDEA 
2. Create separate packages for controller classes, service classes, entity classes, and dao classes. 
○ Packages in Java 
○ Design Pattern - MVC 
3. Auto download any spring dependencies if needed (Check the color codes in the xml files- if the color is red, you need to import the dependency). 
○ Import Spring Dependencies 
4. Create a schema in the database and add a new table. The table should consist of the below column names - 
○ Id (number)

○ First name (only string) 
○ Last name (only string) 
○ Email (valid email with @ sign) 
Congratulations!!! You have completed creating your first Spring MVC project! 
References 
• Creating a new table on SQL 
Bring It On! 
Id is auto-incremental. You can also go for a randomly generated id. Research a bit to know how you can generate random uids (unique-identifiers). 
Expected Outcome 
If everything is successful, We will have the table created in the MySQL/Oracle database and a maven project being set up. 
 3 
Creating the JSP pages using HTML and CSS 
JSP or Java Server Pages is a server-side technology. It is used for creating web applications. It is used to create dynamic web content. In this, JSP tags are used to insert JAVA code into HTML pages. Check out more on Java Server Pages- JSP documentation 
Requirements 
1. Create two JSP pages- 
○ Home page 
○ Customer form 
2. Attributes present in Home page- 
○ Project name as header (CRM - Customer Relationship Manager) ○ Add Customer button (To add the customer information) 
○ View of already added customers (if any) in a table format 
○ Update and Delete link/button on the right side of each customer information 3. Attributes present in Customer Form page- 
○ Project name as header (CRM - Customer Relationship Manager) ○ Input fields for First name, Last name and email address 
○ Save button to save all information 
○ Back button to go back to the home page 
4. Design templates for the two pages- 
○ Home page

○ Add Customer 
○ After Adding 
Congratulations!!! You have completed creating the front-end of this web application!

References 



We can design your own JSP page. However, the functionalities should be the same.
 Expected Outcome 
Run the jsp file in the browser to check the output 
 4 
Creating entity class 
A JPA entity class is a POJO (Plain Old Java Object) class, i.e. an ordinary Java class that is marked (annotated) as having the ability to represent objects in the database. The only unique JPA addition is the @Entity annotation, which marks the class as an entity class. Check out the use of Persistent Fields in entity classes. 
Requirements 
1. Create the entity java class under the entity package. 
2. Import the java persistence API library packages (if not auto-downloaded). Check below to find more about JPA imports- 
○ JPA Dependencies 
3. Write the code in the entity java class to create a POJO class. 
Congratulations!!! You have completed creating the entity class using JPA! 
References 
• Java Persistence API 
Expected Outcome 
The objects created in the entity class should be aligned with the columns in the database. 
 5 
Create Object-Relational Mapping (ORM) connectivity 
Java is one of the most powerful and popular server-side languages in the current scenario. One of the main features of a server-side language is the ability to communicate with the databases. There are two ways of connecting to the database - JDBC and Hibernate (using the ORM framework).

Object Relational Mapping (ORM) is a programming ability to convert data from object type to relational type and vice versa. The main feature of ORM is mapping or binding an object to its data in the database. While mapping we have to consider the data, type of data and its relations with its self-entity or entity in any other table. 
Requirements 
1. Create a package and a class inside it for the ORM connection. 
2. Import the javax servlet library packages (if not auto-downloaded). Check below to find more about javax servlet imports- 
○ Java Servlet API Dependencies 
3. Write the code in the ORM java class. Check how to create an ORM class- ○ Create ORM Class 
4. Provide the JDBC URL and driver path. 
5. Similarly provide the connection details, i.e.- username and password. 
Congratulations!!! You have completed the ORM connection! 
References 
• Java Servlet API Documentation 
• JDBC vs ORM 
Tip 
We can use an online database builder as well. For that, you don't need to install any MySQL Workbench or Oracle SQL Developer for that instance. Check it out - Online Database 

We can also use a file to write and read data instead of using any database. For this, you don't need any ORM connectivity. Find it out! 
Expected Outcome 
On success, your web project will be connected to the database you are working with 
 6 
Create a controller to handle requests and responses 
In Spring MVC, a controller class is written to handle requests coming from the client. Then, the controller invokes a business class to process business-related tasks and then redirects the client to a logical view name, which is resolved by Spring's dispatcher servlet in order to

render results or output. Spring Controller annotation is typically used in combination with annotated handler methods based on the RequestMapping annotation. 
Requirements 
1. Create a controller class under the controller package. 
2. Create five methods: 
○ For listing the customer details 
○ For adding new customers 
○ For saving the customer details 
○ For updating customer information 
○ For deleting customer information 
3. Listing customers will get the customer details when the home page loads. 4. Adding customers will input the customer details from the front-end to the model. (Check out more on the MVC framework) 
5. The save option will save the customer details and return back to the home page. 6. The update option will pre-populate the customer form with information regarding that particular customer so that the user can update. 
7. The delete option will permanently delete the record from the database. Use a dialog box pop up when a user wants to delete a candidate. 
Design functionality for updation and deletion- 
• Before Update 
• Update Page

• After Updation 
• Delete details

• After deletion 
Congratulations!!! You have successfully completed the controller! 
References 
• Web Content with Spring MVC 
• Spring Controllers 
Expected Outcome 
On success, your web project will be able to handle the CRUD operation requests.

 7 
Creating service classes 


The service layer is there to provide logic to operate on the data sent to and from the DAO and the client. Very often these two pieces are bundled together into the same module. The service layer provides code modularity and can also be used to serve loose coupling in the application. 
Requirements 
1. Create a service interface and a service implementation class under the service package. 
2. Write the four method definition on the interface class- 
○ Get the total customer list 
○ Save customer information 
○ Get the customer list from a given customer id (for update functionality) ○ Delete customer information 
3. Write down the service implementation class by defining the four methods implemented from the interface. 
Congratulations!!! You have successfully completed the service class! 
References 
• Use of Service Layer 
• Annotations in Spring 
Tip 
Spring creates proxies for all the classes annotated with @Transactional – either on the class or on any of the methods. Check it out! 
Expected Outcome 
On success, your web project will be able to create an interface that defines the functionality provided by the service. 
 8 
Creating data access object classes 
DAO stands for Data Access Object. It’s a design pattern in which a data access object (DAO) is an object that provides an abstract interface to some type of database or other

persistence mechanisms. By mapping application calls to the persistence layer, DAOs provide some specific data operations without exposing details of the database. While developing a web application, one of the most important aspects is to deal with the database like connection management and transaction management. 
Requirements 
1. Create a dao interface and a dao implementation class under the dao package. 2. Write the four method definition on the interface class as given in the service class. 3. Write down the dao implementation class by defining the four methods implemented 
from the interface. Use hibernate to create the queries. Check out the use of hibernate- ○ Hibernate Queries 
Congratulations!!! You have successfully completed the dao class! 
References 
• Data Access Object pattern 
Bring It On! 
Files can also be used to store and retrieve data. You don't need hibernate queries to fetch them. Check out the use of file writers! 
Expected Outcome 
On success, your web project is finally complete! Complete the next task to run your web application! 
 9 
Run the web application on localhost 
After several hours of design, coding, and testing, your application is ready to be published. As it is a web application, it requires an HTTP server to host it. Apache Tomcat server will manage to do it. It’s an open-source program that processes HTTP requests to access the files stored within a server. These files can be static (it means that whenever a client asks for them they will be shared as they are) or dynamic (before sending files to the client they are generated by the software hosted on a server). In short, Tomcat handles communication via HTTP protocol and delegates requests to the Spring MVC application. 
Requirements 
1. Build the project. There are two ways to build a project- 
○ From the IDE terminal 
○ From the CMD

Open the command (CMD) terminal. Go to the path where the project is residing. Run the below command 
mvn clean install



2. Create a WAR file. If built from IDE. You need to manually build a war file. ● Create a WAR file 
3. Run the tomcat server from IDE or independently 
● From IDE. Define and run application server 
Else keep the WAR file on the tomcat webapps folder and click on start.bat file present in the bin folder. 
● Deploy web application through Tomcat 

Congratulations!!! Your application is running successfully! 
Expected Outcome 
Customer Relationship Management web application is finally running on your local machine!
