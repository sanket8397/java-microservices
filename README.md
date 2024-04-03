# Spring Boot Microservices Project

This is a comprehensive microservices project built using Spring Boot, showcasing various technologies and architectural patterns. The project demonstrates the implementation of microservices, service discovery, API gateway, circuit breakers, distributed tracing, event-driven architecture, containerization, and monitoring.

## Architecture Overview

The project follows a microservices architecture with the following components:

### API Gateway

Implemented using Spring Cloud Gateway, the API Gateway acts as a single entry point for all client requests, intelligently routing them to the appropriate microservices.

### Service Discovery

Netflix Eureka is utilized for service registration and discovery, enabling microservices to locate and communicate with each other dynamically.

### Microservices

1. **Product Service**: Responsible for managing product-related operations.
2. **Order Service**: Handles order-related functionality.
3. **Inventory Service**: Manages inventory-related operations.
4. **Notification Service**: Notifies user after order is complete.

### Authentication

Keycloak is integrated for authentication and authorization purposes, ensuring secure access to microservices.

### Circuit Breaker

Resilience4J is implemented to provide resilience and fallback mechanisms for service communication, ensuring graceful handling of failures.

### Distributed Tracing

Zipkin is employed for distributed tracing, offering visibility into the flow of requests across microservices, aiding in troubleshooting and performance optimization.

### Event-Driven Architecture

Apache Kafka serves as the backbone for event-driven communication between microservices, enabling asynchronous and decoupled interactions.

### Containerization

Docker is utilized for containerizing the microservices, facilitating easy deployment, scaling, and portability across environments.

### Monitoring

Prometheus and Grafana are used for monitoring the microservices, collecting metrics, and visualizing performance data, allowing for effective management and optimization of the system.

## Getting Started

To set up and run the project locally, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Ensure that Docker is installed and running.
4. Use Docker Compose to spin up the microservices and supporting components.

```bash
docker-compose up -d
