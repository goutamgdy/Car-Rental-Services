# 🚗 Car Rental Service

This is a **full-stack Car Rental Service** application that allows users to **browse, book, and manage car rentals** efficiently. The platform provides a seamless experience for **customers, car rental agencies, and administrators** with features like **user authentication, agency registration, and payment integration.**

---

## 🌟 Features  
- **User Authentication** – Secure login and registration using JWT.  
- **Role-Based Access Control** – Separate dashboards for Customers, Agencies, and Admins.  
- **Car Search & Booking** – Filter cars by city, category, and availability.  
- **Agency Management** – Register, update, and manage agency profiles and cars.  
- **Payment Integration** – Secure payment gateway integration.  
- **Microservices Architecture** – Using Spring Cloud Gateway and Discovery for routing and service registry.  
- **Responsive UI** – Built with React for a dynamic and user-friendly experience.  

---

## 🛠️ Tech Stack  
### **Frontend**  
- **React** – For building a dynamic and responsive UI.  
- **Redux** – State management.  
- **Axios** – For API calls.  
- **React Hook Form** – Form validation and handling.  

### **Backend**  
- **Spring Boot** – Microservices architecture for modular design.  
- **Spring Security** – JWT-based authentication and authorization.  
- **Hibernate** – ORM for database operations.  
- **Spring Data JPA** – For interacting with the database.  
- **Spring Cloud Gateway** – API Gateway for routing requests.  
- **Eureka Discovery** – Service registry and discovery.  

### **Database**  
- **MySQL** – Relational database to store user, car, booking, and payment information.  

### **Build Tools**  
- **Maven** – Dependency management and build automation for Spring Boot.  
- **npm** – Package management for React.  

---

## ⚙️ Dependencies  
### **Frontend (React)**  
```
"axios": "^1.x.x",
"redux": "^4.x.x",
"react-redux": "^7.x.x",
"react-router-dom": "^6.x.x",
"react-hook-form": "^7.x.x",
"bootstrap": "^5.x.x"
```

### **Backend (Spring Boot & Microservices)**  
- **Spring Boot Starter Web** – To build RESTful APIs.  
- **Spring Boot Starter Security** – For JWT authentication.  
- **Spring Boot Starter Data JPA** – ORM integration with Hibernate.  
- **Spring Boot Starter Validation** – For request validation.  
- **Spring Cloud Starter Gateway** – API Gateway.  
- **Spring Cloud Starter Eureka Server** – Service Discovery.  
- **MySQL Connector** – For database connection.  
- **Lombok** – To reduce boilerplate code.  

### **Database (MySQL)**  
- **MySQL 8.x.x** – Database for storing application data.  
- **Database Schema** – Includes tables for Users, Roles, Cars, Bookings, Payments, and Agencies.  

---

## 📁 Folder Structure  
```
car-rental-service/
├── backend/
│   ├── api-gateway/          # Spring Cloud Gateway
│   ├── discovery-server/     # Eureka Discovery Server
│   ├── user-service/         # User management microservice
│   ├── car-service/          # Car and agency management
│   ├── booking-service/      # Booking management
│   └── payment-service/      # Payment integration
└── frontend/
    └── car-rental-frontend/  # React application
```

---

## ⚙️ Configuration  
### **Backend**  
- **application.properties**  
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/car_rental_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
spring.jpa.show-sql=true
jwt.secret=your_secret_key
jwt.expiration=86400000  # 24 hours
eureka.client.service-url.defaultZone=http://localhost:8761/eureka
```

### **Frontend**  
- **.env**  
```env
REACT_APP_API_URL=http://localhost:8080/api
```

---

## 🚀 Getting Started  
### **1. Clone the Repository**  
```bash
git clone https://github.com/yourusername/car-rental-service.git
cd car-rental-service
```

### **2. Database Setup**  
- Create a **MySQL database** named `car_rental_db`.  
- Update the database credentials in `application.properties`.  
- The database schema will be auto-generated using **Hibernate**.  

### **3. Backend Setup**  
```bash
cd backend
./mvnw clean install
```
### **4. Frontend Setup**  
```bash
cd frontend/car-rental-frontend
npm install
npm start
```

---

## 🧪 Testing  
- **Postman** – For API testing.  
- **Jest** – Unit testing for React components.  

---

## 🚧 Challenges Faced  
- **Complex State Management** – Solved using Redux.  
- **API Integration Issues** – Managed with Axios interceptors.  
- **JWT Token Expiry** – Implemented custom logic for token renewal.  

---

## 🔒 Security Measures  
- **JWT Authentication** – Role-based authorization.  
- **Input Validation** – Using Spring Validation.  
- **Password Encryption** – BCrypt for secure storage.  

---

## 📌 Future Enhancements  
- **.NET Microservices** – For better scalability.  
- **Dockerization** – For cloud deployment.  
- **CI/CD Integration** – Using Jenkins or GitHub Actions.  

---

## 📝 License  
This project is licensed under the **CDAC License**.  

---

## 📧 Contact  
For any queries or feedback, feel free to reach out at **goutamgdy@gmail.com**.  

---

