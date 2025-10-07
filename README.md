🛒 Full-Stack E-Commerce Web Application

A modern e-commerce web application built with Spring Boot (Java) for the backend and ReactJS with Vite for the frontend.
This project demonstrates full-stack development, integrating RESTful APIs with a responsive frontend—ideal for learning, demos, or portfolio showcase.

📌 Prerequisites

-Java 17+

-Maven

-Node.js & npm

-MySQL database

-Git (for version control)

📁 Project Structure
SpringBoot-Reactjs-Ecommerce-main/
├── Ecommerce-Backend/       # Spring Boot backend with REST APIs
├── Ecommerce-Frontend/      # ReactJS frontend powered by Vite

🏗️ Backend – Spring Boot

💻 Technologies

-Java 17+

-Spring Boot

-Spring Data JPA

-MySQL

-Maven

📂 Directory Layout

Ecommerce-Backend/
├── controller/       # REST API endpoints
├── model/            # JPA entity classes
├── repo/             # Spring Data JPA repositories
├── service/          # Business logic
├── resources/
│   ├── application.properties  # DB & app config
│   └── data1.sql               # Seed data
└── pom.xml            # Maven build configuration

⚙️ Backend Setup & Run

1)Database Setup

-Create a MySQL database, e.g., ecomdb.
-Update application.properties:
spring.datasource.url=jdbc:mysql://localhost:3306/ecomdb
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update

2)Run Backend

cd Ecommerce-Backend
mvn spring-boot:run


3)Seed Data

-On first run, data1.sql will initialize sample products in the database.

🌐 API Endpoints
|Method |      |Endpoint	|       |   Description    |
GET	           /products	          Fetch all products
GET	          /products/{id}      	Get product by ID
POST        	/products            	Add a new product
PUT	          /products/{id}	       Update product
DELETE      	/products/{id}	       Delete product

🌟 Frontend – ReactJS + Vite

💻 Technologies

-ReactJS

-Vite

-Axios (API requests)

-Bootstrap (UI)

-ES6+ JavaScript

📂 Directory Layout

Ecommerce-Frontend/
├── public/          # Static assets
├── src/
│   ├── components/  # Reusable components
│   ├── pages/       # Page-level components
│   ├── App.jsx      # Main layout
│   └── main.jsx     # Entry point
├── package.json
└── vite.config.js

⚡ Frontend Setup & Run

1)Install dependencies

cd Ecommerce-Frontend
npm install


2)Start Frontend

npm run dev

Access the frontend at: http://localhost:5173

3)Connect to Backend

-Update API URLs in frontend service files if needed:

axios.get('http://localhost:8080/products')

🛍️ Features

-Fetch and display product list dynamically

-Fully responsive UI design

-Integration-ready for cart, checkout, login, and more

-Clear separation of backend and frontend logic

-Easy to extend with new functionalities

🔧 Future Improvements

-Add user authentication (JWT / OAuth)

-Implement shopping cart & order checkout

-Add search & filtering functionality

Deploy to cloud platforms (Heroku, Vercel, Netlify)

Enhance UI/UX with animations or modern design frameworks
