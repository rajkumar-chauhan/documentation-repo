# SALARY API  

| AUTHOR |CREATED ON |
|--------|-----------|
|RAJKUMAR| 05-06-2024|

## Purpose 
We need an Api microservice which is responsible for storing all the salary related transactions and records of Employee in [OT-Microservices](https://github.com/OT-MICROSERVICES) stack. This Application is must be independent and can be run on multiple operating system. JAVA RUNTIME would be required to run this application.

## Pre-requisites
The Salary API application have some database, cache manager and package dependencies. Ensure you have the following on your system :
* ScyllaDB
* Redis
* Maven
* Migrate

## System Requirements 
|Hardware Specification |Minimum Recommendation|
|:-----------------------:|:----------------------:|
|Processor              | Dual-core            |
|RAM                    | 4GB                  |
|Disk                   | 20GB                 |
|OS                     |Ubuntu(22.04)         |

## Build-Time Dependency
| Name | Version | Description |
|:-----:|:------:|:------------:|
|Maven|3.+|It helps manage project dependencies, build processes, and project documentation.|

## Run-Time Dependency
|Name  | Version | Description |
|:------:|:-------:|:----------:|
|JAVA|  17| It is necessary to run the compiled Java application.|

## Architecture 

![Salary API](https://github.com/OT-MICROSERVICES/salary-api/blob/main/static/salary.png)

## Dataflow 

### Client Requests:
The process begins when a client (such as a web application, mobile app, or any other consumer) sends a request to the Salary API. These requests can be for various operations like creating a new salary record, retrieving salary data, updating existing records, or deleting them.

### API Gateway/Controller:
The requests are received by the API Gateway or the controller layer of the Salary API. This layer is responsible for routing the requests to the appropriate service. It also handles authentication, authorization, and request validation.

### Service Layer:
The controller forwards the request to the service layer, which contains the business logic. The service layer processes the request, applying necessary business rules and logic. For example, it might calculate bonuses, apply tax rules, or validate salary caps.

### Database Interaction:
The service layer will interact with database:
**ScyllaDB**: For operations requiring high performance and low latency, such as real-time data processing, ScyllaDB is used. It might store frequently accessed data or handle operations that require fast read/write capabilities.


### Data Retrieval/Modification:
The service layer sends queries to the respective database (ScyllaDB ) to retrieve or modify data.
Read Operations: For read operations, the data is fetched from the database, processed if necessary, and then sent back up through the service layer to the controller.
Write Operations: For write operations, the data is validated and then saved to the appropriate database. The result of the operation (success or failure) is sent back through the service layer to the controller.

### Response to Client:
The controller constructs a response based on the service layer's output and sends it back to the client. This response could be the requested data, a confirmation of a successful operation, or an error message if something went wrong.

## Setting Up the Environment
**ScyllaDB**
Install ScyllaDB
To install ScyllaDB, execute the following commands:
```
curl -sSf get.scylladb.com/server | sudo bash
sudo scylla_io_setup
```
**Redis**
Install Redis
To install Redis, use the following commands:
```
 sudo apt install redis-server
 sudo systemctl start redis-server
 sudo systemctl status redis-server
 redis-cli
 ping
```
### Required Libraries
**Install JDK 17**
To install JDK 17, run:
```
sudo apt install openjdk-17-jdk
```
**Install Maven**
To install Maven, execute:
```
sudo apt install maven
```
**Install Migrate**
To install Migrate, use the following commands:
```
curl -L https://github.com/golang-migrate/migrate/releases/download/v4.15.2/migrate.linux-amd64.tar.gz -o migrate.tar.gz
tar -xvzf migrate.tar.gz
sudo mv migrate /usr/local/bin/
sudo chmod +x /usr/local/bin/migrate
```
## Building and Running the Salary API
### Skip Test Cases and Build
To build the project and skip test cases, execute:
```
mvn clean package -Dmaven.test.skip=true
```
### Testing
**Checkstyle**
To run Checkstyle, use:
```
mvn checkstyle:checkstyle
```
**Run Tests**
To run the test cases, execute:
```
mvn test
```
### Running the Java Application
To run the Java application, navigate to the project directory and use the following command:
```
java -jar target/salary-api.jar
```
## Conclusion
Following these steps, you will set up the necessary environment for the Salary API, build the project, and run the application. Ensure that all commands are executed in the correct order and in a terminal with sufficient privileges.
Other Endpoint are below 


## References 
|links | Description |
|-------|------------|
|https://redis.io/docs/latest/operate/oss_and_stack/install/install-redis/install-redis-on-linux/|For Redis |
|https://opensource.docs.scylladb.com/stable/getting-started/install-scylla/install-on-linux.html| For Scylladb|
|https://github.com/OT-MICROSERVICES/salary-api|For understanding the workflow of salary api|



## Contact Information 
|Name|Email Address|
|:---:|:---:|
|Rajkumar|rajchauhan9584@gmai.com|





