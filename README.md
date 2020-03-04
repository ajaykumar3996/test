
#Batchman

##Description

The Basic idea is to provide ability to handle batch operations for JIRA Issues like moving JIRA’s between different servers or changing the status or comments on JIRA. 

Refer this [link](https://jira2.cerner.com/browse/ACADEM-54122) to know more

##Project Setup

This Project requires 

Download and install [Intellij IDEA](https://www.jetbrains.com/idea/download/)

Download and install [Oracle JDK 8u241](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html)

Download and install    [Maven 3.6.3](https://maven.apache.org/download.cgi) 


Download and install [Node and npm]( https://nodejs.org/en/download/) and install the Recommended for Most Users version

Download and install [Git 2.25.1]( https://git-scm.com/downloads)

Download and install [Webstorm]( https://www.jetbrains.com/webstorm/download/#section=windows)

This project makes use of [JIRA API]() 

##### Clone the Repository

1. Create a folder for the repository, open git bash, and navigate to that folder

2. Clone the repository using: 

```sh
git clone https://github.training.cerner.com/DevCenter/Batchman.git
```


You can verify the installation of all of these on the command line using:

```sh
java -version
```
```sh
mvn -version
```
```sh
npm -version
```
```sh
node -v
```
```sh
ng version
```

##### Install Postman

Navigate to the website for [Postman](https://www.getpostman.com/downloads/) and download the latest version for your system (most likely 64 bit windows)

Follow the setup instructions they provide in the setup

#### Manual Testing the API Endpoints

[Postman](https://www.getpostman.com/downloads/) will help with testing the endpoints and viewing what kind of data the backend expects as well as what kind of data will be returned and how it will look.

To use Postman: 

1.  Open up the Postman application

2.  Click the orange button in the upper left corner marked New

3.  Select Request.  This will generate an empty GET request
    3a. To change the request type, click on the GET with the dropdown arrow that precedes the URL area

4.  Find a Request in any of the backend controller files that accepts the type of request you are sending (which can be any of the following GET, PUT, POST, or DELETE)

5.  Fill out the URL for the controller endpoint (will typically start with http://localhost:8080/api/v1 followed by the URL in the controller)

6.  Click send
    6a.  If you are doing a POST or PUT request, you may have to fill out additional information

7.  In the Response window of Postman will be the returned results from your request

##### Running the Project

JAR file can be created by doing a maven build (right-click project folder -> run as -> maven build) *Note if prompted for maven goals enter:

```sh 
mvn clean install -U
```

App can be run directly by running as a Spring Boot app. The spring plugin stated above is needed to do this.

Right click project folder -> run as -> Spring Boot App

The app can also be run in the command line by navigating to the directory of the project and running the command:

```sh
mvn exec:java
```

