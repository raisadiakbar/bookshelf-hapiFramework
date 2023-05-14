#Bookshelf App using Hapi Framework
This is a simple bookshelf app built using Hapi Framework, PostgreSQL as database, and Sequelize as ORM. This app allows users to create, read, update, and delete books from the bookshelf. It also has authentication and authorization features for managing users.

###Requirements
Node.js version 14 or above
PostgreSQL

###Installation
Clone this repository
Run npm install to install the dependencies
Create a .env file based on .env.example and set the database connection details
Run npm run migrate to create the database tables
Run npm run seed to seed the database with sample data (optional)
Run npm start to start the server
Open http://localhost:3000 on your browser to access the app

##API Documentation

###Authentication Endpoints
POST /auth/register: Register a new user
POST /auth/login: Login with existing user
POST /auth/logout: Logout the currently logged in user

###Book Endpoints
GET /books: Get all books
GET /books/{id}: Get a book by its ID
POST /books: Create a new book
PUT /books/{id}: Update an existing book by its ID
DELETE /books/{id}: Delete a book by its ID

###User Endpoints
GET /users: Get all users (requires admin privileges)
GET /users/{id}: Get a user by its ID (requires admin privileges)
PUT /users/{id}: Update a user by its ID (requires admin privileges)
DELETE /users/{id}: Delete a user by its ID (requires admin privileges)

##Request and Response Examples
Please refer to the example.http file for request and response examples.
