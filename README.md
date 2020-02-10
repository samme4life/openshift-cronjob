# openshift-cronjob
SpringBatch spike: YAML file which contains cronjob information to be imported into OpenShift project
User Registration API
This codebase is to implement an API to register a user, it can also edit/read/soft delete (deactivate) single or multiple user(s)

The API Document can be found at "https://app.swaggerhub.com/apis/samme4life/user-rego/0.0.1"

To Run using Docker
This service can be run in a Docker container Steps to follow,

mvn clean package - this command will create the jar file

docker build -t user-rego . - this command will create the docker image using the jar file

docker image ls - this will list down the docker images to make sure it is created in the previous step

docker run -p 5000:8080 user-rego - this will run the docker image mapped to localhost's port 5000. for example you can now see the app's status by hitting "http://localhost:5000/user/status"

Technical Overview
This project was generated with

Spring Boot 2.1.2
Java 1.8
In order to implement the data layer, H2 In Memory DB is used

to access the h2 console [URL] (/h2)
login details are as follows,
JDBC URL: jdbc:h2:file:~/user
User Name: sa
(It is not password protected)
Running the Applicaton Locally
clone the repo using the command "git clone https://github.com/samme4life/user-rego.git"
download and install Maven 3 (http://maven.apache.org/download.html#Installation). If you have already installed Maven 3, you can skip this step.
go to the root directory of the project (where the pom.xml file is)
run command "mvn spring-boot:run"
the project will be deployed at http://localhost:8080 meaning,
to get the service status the URL is: http://localhost:8080/user/status
Running unit tests
unit tests can be run using this command: mvn test
To-Do
Password Encryption
Improve API Doc
More unit tests to cover more positive and negative paths
