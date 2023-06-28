# Eureka Server Application

You can think of it as a structure that keeps a list of applications running on the platform. Each microservice application registers itself to Eureka Server. Eureka Server has a mechanism that periodically sends requests to applications and checks whether they are alive or not. If the application is not standing, it is automatically deleted from the list.


## If you want to run it with Docker

### Build: 
docker build -t sehmusaydogdu/eurekaserverapp .

### Run:   
docker run -p 8761:8761 sehmusaydogdu/eurekaserverapp

### Stop:  
docker stop <containerId>

## If you want to run it with Maven
mvn spring-boot:run