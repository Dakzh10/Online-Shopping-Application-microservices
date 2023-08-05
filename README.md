
# Online Shopping Application Microservices

Built an Online Shopping Application with key features:

1. Service Discovery.
2. Centralized Distribution.
3. Distributed Tracing.
4. Event Driven Achitecture.
5. Centralized Logging.
6. Circuit Breaker Design Architecture.
7. Secured Microservices using KeyCloak.


[![image](https://www.linkpicture.com/q/Screenshot-from-2023-07-29-13-08-46.png)](https://www.linkpicture.com/view.php?img=LPic64c4c2d7741d91725894923)


## Project Description:

 
SPRING CLOUD PROJECT OVERVIEW:

The main module which helps us to write microservices using Spring Framework is Spring Cloud, in this tutorial series, we are going to mainly concentrate on the following modules which are part of Spring Cloud:

    Spring Cloud Config Server
    Spring Cloud Bus
    Spring Cloud Netflix Eureka
    Spring Cloud Circuit Breaker
    Spring Cloud Sleuth
    Spring Cloud Gateway
    Spring Cloud Stream

SPRING CLOUD CONFIG SERVER

This module is used to externalize the configuration of our microservices into a centralized place.

If there are any changes in the configuration, our applications should be updated without the need to restart them.

There are many options to implement this Centralized Configuration eg: Using a Git Repository, or using HashiCorp Consul etc.

We are also going to use HashiCorp Vault as one of the backends to maintain the secrets for our application.

SPRING CLOUD BUS

This module contains a light weight message broker implementation, which is mainly used to broadcast some messages to the other services.

In our project, we will use this module, to broadcast configuration changes in our Config Server.

SPRING CLOUD NETFLIX EUREKA

This module is used to implement the Service Registry and Discovery Pattern in Microservices architecture.

As there can be many independent Microservices, we need a reliable way to scale the services and provide inter-service communication instead of hard-coding the service information.

SPRING Cloud  Netflix Eureka module uses Netflix’s Eureka library to provide this functionality.


SPRING CLOUD CIRCUIT BREAKER

Inter-service Communication is common in the Microservice architecture, if one of the service is down, the other service which is communicating with it, should be able to handle this failure gracefully.

Spring Cloud Circuit Breaker provides an abstraction over different Circuit Breaker implementations like Reslience4J, Hystrix, Sentinel etc.

In our project, we are going to use Spring Cloud Circuit Breaker with Resilience4J

SPRING CLOUD SLEUTH

In Microservice Architecture, if there is any error, it’s hard to debug and trace it, Spring Cloud Sleuth provides us with the functionality to trace the inter-service calls.

SPRING CLOUD GATEWAY

This library helps us to implement the API Gateway pattern, by hiding the complexity of our microservices from the external clients.

If a client want’s to connect to one of our services, all the traffic will be going through the API Gateway and the gateway will route the request to the appropriate service.

This library also handles the cross-cutting concerns like Security, Monitoring, Rate-limiting and Resiliency.

We will secure our microservices using Keycloak as Authorization Server together with the Spring Cloud Gateway.

SPRING CLOUD STREAM

This module mainly allows us to implement asynchronous communication between our microservices using event-driven architecture.

We are going to use RabbitMQ as a message broker to implement some event driven microservices.

DISTRIBUTED LOGGING using ELK STACK

Even though, this is not part of the Spring Cloud Stack, we are going to implement Centralized Logging for our microservices using ELK Stack (Elasticsearch, Logstash and Kibana)

