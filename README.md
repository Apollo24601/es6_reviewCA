# ES6 Backend API with MongoDB

 Project Overview

This project is a backend API built using modern **ES6 JavaScript features**. It uses **Node.js**, **Express**, and **MongoDB (via Mongoose)** to implement a simple CRUD (Create, Read, Update, Delete) system for managing users.

Technologies Used

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* dotenv
* CORS


 Project Setup

1. Created a project folder and initialized it using:

   ```bash
   npm init -y
   ```

2. Installed required dependencies:

   ```bash
   npm install express mongoose cors dotenv
   ```

3. Enabled ES6 modules by adding:

   ```json
   "type": "module"
   ```

 Environment Configuration

* Created a `.env` file to store sensitive data:

  ```env
  MONGO_URI=your_mongodb_connection_string
  PORT=5000
  ```

* Added `.env` to `.gitignore` to prevent exposing credentials.


 MongoDB Integration

* Created a MongoDB Atlas cluster.
* Configured database user and network access.
* Connected the application to MongoDB using Mongoose.


🧩 Application Structure

* `app.js` → Main server file
* `.env` → Environment variables
* `.gitignore` → Ignored sensitive/system files

 Features Implemented

 1. Express Server

* Set up an Express server
* Configured middleware (`express.json()`, `cors()`)

 2. Mongoose Model

* Defined a `User` schema with:

  * `name`
  * `age`

3. CRUD Operations

* **Create User (POST)**
  `/users`

* **Get All Users (GET)**
  `/users`

* **Update User (PUT)**
  `/users/:id`

* **Delete User (DELETE)**
  `/users/:id`

Testing

* Tested endpoints using Postman
* Verified all CRUD operations:

  * Data creation
  * Data retrieval
  * Data updates
  * Data deletion

Deployment

* Code pushed to GitHub
* Prepared for deployment using Render
* Environment variables configured for production

* Understanding of ES6 modules (`import/export`)
* Building RESTful APIs with Express
* Connecting Node.js applications to MongoDB
* Using Mongoose for schema and data modeling
* Managing environment variables securely
* Using Git and GitHub for version control
* Debugging real-world backend issues


This project demonstrates the development of a fully functional backend API using modern JavaScript tools and practices. It highlights the integration of ES6 features, database connectivity, and RESTful API design.
