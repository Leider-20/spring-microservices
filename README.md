# Spring Microservices

Microservices-based backend project built with Java and Spring ecosystem, focused on scalable service communication, centralized configuration, and API routing.

## Overview

This repository contains a microservices architecture implementation using Spring Boot and Spring Cloud components. The project is structured to simulate a distributed backend environment where services communicate independently while remaining connected through discovery, configuration, and gateway layers.

## Architecture

The system is composed of:

- **Config Server** → Centralized configuration management
- **Eureka Server** → Service discovery and registration
- **API Gateway** → Single entry point for all client requests
- **Student Service** → Student management microservice
- **Course Service** → Course management microservice
- **Feign Client** → Inter-service communication

## Project Structure

```bash
spring-microservices/
│── microservice-config/
│── microservice-eureka/
│── microservice-gateway/
│── microservice-student/
│── microservice-course/
│── pom.xml
```

## Tech Stack

- Java 17
- Spring Boot
- Spring Cloud
- Spring Cloud Gateway
- Eureka Server
- OpenFeign
- PostgreSQL
- MySQL
- Maven

## Service Flow

Client Request  
↓  
API Gateway  
↓  
Eureka resolves target service  
↓  
Microservice execution  
↓  
Feign communication (if another service is required)  
↓  
Database interaction  
↓  
Response

## Features

- Distributed architecture
- Centralized configuration
- Dynamic service discovery
- API Gateway routing
- Inter-service communication with Feign
- Independent service deployment
- Database integration (MySQL / PostgreSQL)

## Running the Project

Start services in this order:

1. **microservice-config**
2. **microservice-eureka**
3. **microservice-gateway**
4. **microservice-student**
5. **microservice-course**

Then access endpoints through the Gateway.

## Learning Goals

This project was built to practice:

- Microservices architecture
- Service registration/discovery
- API Gateway patterns
- Distributed configuration
- Inter-service communication
- Spring Cloud ecosystem

## Author

Developed by **Leider Felipe**
