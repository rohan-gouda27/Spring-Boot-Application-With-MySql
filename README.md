This is a **Spring Boot** project that provides a **CRUD (Create, Read, Update, Delete) REST API** for managing products. It uses **Spring Boot, Spring Data JPA, and MySQL** as the database.
---
## 🚀 Features

- 📌 Create a new product  
- 📌 Get all products  
- 📌 Get a product by ID  
- 📌 Update a product  
- 📌 Delete a product  
- 📌 MySQL database integration  
- 📌 Uses Hibernate & Spring Data JPA  

---

## 🛠️ Technologies Used

- **Java 21**  
- **Spring Boot 3.4.2**  
- **Spring Data JPA (Hibernate)**  
- **MySQL Database**  
- **Maven**  
- **Postman for API Testing**

---

## 📦 Project Structure

```
spring-boot-crud/
│-- src/main/java/com/example/product/
│   ├── controller/       # REST API Controllers
│   ├── entity/           # JPA Entities (Database Models)
│   ├── repository/       # Spring Data JPA Repositories
│   ├── service/          # Business Logic Layer
│   ├── SpringBootCrudApplication.java  # Main Application File
│-- src/main/resources/
│   ├── application.properties  # Database Configuration
│-- pom.xml  # Maven Dependencies
```

### 2️⃣ **Set Up MySQL Database**
- Open **MySQL Workbench** and create a database:
```sql
CREATE DATABASE product_db;
```
- Update your **application.properties** file:
```properties
spring.datasource.url=jdbc:mysql://127.0.0.1:3306/product_db?useSSL=false&allowPublicKeyRetrieval=true
spring.datasource.username=root
spring.datasource.password=your_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update
```

### 3️⃣ **Run the Application**
```sh
mvn spring-boot:run
```

---

## 📡 REST API Endpoints

| Method | Endpoint         | Description             |
|--------|----------------|------------------------|
| `POST` | `/products`     | Add a new product      |
| `GET`  | `/products`     | Get all products      |
| `GET`  | `/products/{id}` | Get product by ID     |
| `PUT`  | `/products/{id}` | Update product by ID  |
| `DELETE` | `/products/{id}` | Delete product by ID |

---

## 🧪 Test API with Postman

1️⃣ **Start the Spring Boot application**  
2️⃣ **Open Postman** and send requests to:
   - `GET http://localhost:8080/products`
   - `POST http://localhost:8080/products` (with JSON body)
   - `PUT http://localhost:8080/products/{id}`
   - `DELETE http://localhost:8080/products/{id}`

---
## 🎯 Contributing
If you'd like to contribute, feel free to open a pull request. 🚀

---

### 📌 Author
👨‍💻 **Rohan Gouda**  
📧 rohan.g0126@gmail.com  
🔗 [GitHub Profile](https://github.com/rohan-gouda27)

```
