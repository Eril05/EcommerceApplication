# EcommerceApplication

This project is a backend solution for an e-commerce platform. It is built with a microservices architecture, where each service is dedicated to a specific functionality, ensuring modularity, scalability, and ease of maintenance.

## Microservices Overview

Below is an overview of each microservice repository in this application.

### 1. **[Product Service](https://github.com/Eril05/ProductService.git)**
- **Functionality**: Manages product-related operations, including CRUD operations on product data.
- **Responsibilities**:
  - Add, update, delete, and view products.
  - Manage product categories and details.
  
### 2. **[User Service](https://github.com/Eril05/UserService.git)**
- **Functionality**: Handles user authentication, registration, and authorization.
- **Responsibilities**:
  - User sign-in, login, and registration.
  - Token-based authentication using OAuth2.
  - Secure endpoints and user session management.

### 3. **[Service Discovery (Eureka Server)](https://github.com/Eril05/ServiceDiscovery.git)**
- **Functionality**: Acts as a service registry for the microservices using Spring Cloud Eureka.
- **Responsibilities**:
  - Enables service discovery between various services in the application.
  - Provides a registry of services and their instances for load balancing and fault tolerance.

### 4. **[API Gateway](https://github.com/Eril05/ApiGateway.git)**
- **Functionality**: Works as an API Gateway, routing incoming client requests to the appropriate services.
- **Responsibilities**:
  - Acts as a reverse proxy for incoming requests.
  - Implements load balancing for downstream services.

### 5. **[Payment Service](https://github.com/Eril05/PaymentService.git)**
- **Functionality**: Generates payment links to Razorpay for processing payments.
- **Responsibilities**:
  - Generates payment URLs by integrating with the Razorpay API.
  - Redirects the user to Razorpay’s payment gateway for transaction processing.
  - Returns the status of the payment transaction once completed.
  - Handles payment-related callbacks and updates order statuses accordingly.
  
### 6. **[Email Service](https://github.com/Eril05/EmailService.git)**
- **Functionality**: Sends email notifications based on specific events in the system.
- **Responsibilities**:
  - Sends event-driven email notifications (e.g., Welcome mail).
  - Integrates with SMTP or third-party email providers for delivery.

## Technologies Used

- **Spring Boot** for building the backend services.
- **Spring Cloud** for microservice communication and service discovery.
- **Eureka Server** for service registry and discovery.
- **Kafka** for asynchronous communication.
- **Redis** for caching and improving response time.
- **OAuth2** for secure authentication and authorization.
- **AWS** for deploying services on the cloud.
- **Razorpay API** for payment gateway integration.
