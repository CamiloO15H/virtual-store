# Virtual Store

## Overview
This is a Java Spring Boot application for a virtual store that allows users to browse a catalog of serum products and make purchases. The application provides a simple interface for product visualization and management.

## Features
- View a catalog of serum products
- Retrieve product details by ID
- Basic CRUD operations for products

## Project Structure
```
virtual-store
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── virtualstore
│   │   │           ├── VirtualStoreApplication.java
│   │   │           ├── controller
│   │   │           │   └── ProductController.java
│   │   │           ├── model
│   │   │           │   └── Product.java
│   │   │           ├── repository
│   │   │           │   └── ProductRepository.java
│   │   │           └── service
│   │   │               └── ProductService.java
│   │   └── resources
│   │       ├── application.properties
│   │       └── data.sql
│   └── test
│       └── java
│           └── com
│               └── virtualstore
│                   └── VirtualStoreApplicationTests.java
├── pom.xml
└── README.md
```

## Setup Instructions
1. **Clone the repository:**
   ```
   git clone <repository-url>
   cd virtual-store
   ```

2. **Build the project:**
   ```
   mvn clean install
   ```

3. **Run the application:**
   ```
   mvn spring-boot:run
   ```

4. **Access the application:**
   Open your web browser and navigate to `http://localhost:8080`.

## Usage
- Use the endpoints provided by the `ProductController` to interact with the product catalog.
- The application initializes with sample product data defined in `data.sql`.

## Dependencies
- Spring Boot Starter Web
- Spring Boot Starter Data JPA
- Database driver (e.g., H2, MySQL)

## License
This project is licensed under the MIT License.