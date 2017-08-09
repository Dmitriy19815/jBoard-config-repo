# jBoard-config-repo
The remote bucket for storing and serving distributed configurations across multiple applications and environments

This supposed to use with Spring Cloud Bus smart opportunities throught of the service application for distribute custom parameters from once node.


## How to run ?

Keep in mind, that you are going to start 8 Spring Boot applications and RabbitMq.


#### Before you start
- Install Docker and Docker Compose (quite important).

- Create docker network: run in command shell `docker network create jBoardNetwork_default`
    

#### Development mode
    
If you'd like to build images yourself (with some changes in the code, for example), you have to clone all repository and build artifacts with gradle.
Then, run `docker-compose -f docker-compose.yml up --build`


#### Important endpoints
- http://localhost:8888/admin/info - managed endpoint for entry to service
