# E-commerce Backend System

This project is a simple e-commerce backend system designed to demonstrate a microservices architecture using .NET, Docker, and Nginx. The system is composed of three main microservices: Catalog (Product) Service, Order Service, and Identity (User) Service. Each service operates independently, managing its domain-specific operations and data.

## Architecture Overview


### Architecture Components

- **Nginx**: Serves as the entry point for all incoming requests. It acts as a reverse proxy and load balancer, routing requests to the appropriate microservice based on the URL path.

- **Microservices**:
  - **Catalog Service**: Manages product information and inventory.
  - **Order Service**: Handles order creation, updates, and status tracking.
  - **Identity Service**: Responsible for user registration, authentication, and user management.

- **Database**: Each microservice utilizes its database to ensure decoupling and data encapsulation. For development, SQLite can be used for its simplicity, whereas PostgreSQL, MySQL, or MongoDB are recommended for production environments, depending on the service requirements.

- **Docker Containers**: The entire system, including microservices and Nginx, is containerized. This approach ensures consistency across different environments and simplifies deployment and scaling processes.

## Getting Started


