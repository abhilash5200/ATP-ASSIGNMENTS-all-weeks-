# ATP WEEK-5

## Advanced Backend Development with Node.js, Express.js & MongoDB

### Overview

This repository focuses on advanced backend development concepts using Node.js, Express.js, MongoDB, and Mongoose. The project demonstrates how real-world backend applications are structured using modular architecture, authentication middleware, database integration, and REST APIs.

By completing this project, developers gain hands-on experience in building scalable and maintainable backend applications.

---

## Technologies Used

### Backend Technologies

- Node.js
- Express.js
- MongoDB
- Mongoose

### Development Tools

- Visual Studio Code
- Git & GitHub
- npm
- REST Client / Postman

---

## Project Structure

```text
ATP WEEK-5/
│
├── APIs/
│   ├── product_api.js
│   └── user_api.js
│
├── middleware/
│   └── verifytoken.js
│
├── models/
│   ├── productmodel.js
│   └── usermodel.js
│
├── server.js
├── package.json
├── package-lock.json
├── req.http
└── .gitignore
```

---

# Main Server

## server.js

The main entry point of the backend application.

### Responsibilities

- Create Express Server
- Configure Middleware
- Connect API Routes
- Manage Requests and Responses
- Start Backend Server

### Concepts Covered

- Express Server Setup
- Middleware Integration
- Route Handling
- API Management
- JSON Parsing

### Example

```javascript
app.use(express.json());

app.listen(PORT, () => {
    console.log(`Server running on port ${PORT}`);
});
```

### Backend Workflow

```text
Client Request
      ↓
Express Server
      ↓
Middleware
      ↓
API Route
      ↓
Database Interaction
      ↓
Response Sent Back
```

### Learning Outcome

Understand how scalable backend servers are built and managed using Express.js.

---

# APIs Folder

The APIs folder contains route handlers organized by functionality to improve maintainability and scalability.

---

## user_api.js

### User API Module

Handles user-related backend operations.

### Features

- User Creation
- User Retrieval
- User Authentication
- User Data Management

### Concepts Covered

- Express Router
- REST APIs
- Request Handling
- Response Handling
- User Management

### Example Route

```javascript
router.get('/users', (req, res) => {
    res.send("Users Data");
});
```

### Workflow

```text
Frontend Request
      ↓
User API Route
      ↓
Process User Data
      ↓
Database Operation
      ↓
Return Response
```

### Learning Outcome

Learn how user-related APIs are developed and organized in backend applications.

---

## product_api.js

### Product API Module

Handles product-related backend operations.

### Features

- Product APIs
- Product Data Management
- Product Routes
- API Responses

### Concepts Covered

- Product Management
- API Routing
- REST Architecture
- Modular Backend Design

### Workflow

```text
Product Request
      ↓
Product API
      ↓
Process Product Data
      ↓
Database Interaction
      ↓
Return Response
```

### Learning Outcome

Understand how product-related APIs are implemented in scalable backend systems.

---

# Middleware Folder

## verifytoken.js

Authentication middleware used to secure protected routes.

### Features

- Token Verification
- Authentication Validation
- Route Protection
- Secure API Access

### Concepts Covered

- Middleware
- Authentication
- Authorization
- Protected Routes

### Middleware Workflow

```text
Client Request
      ↓
Verify Token Middleware
      ↓
Token Valid?
   ↙         ↘
 YES         NO
  ↓           ↓
Continue   Reject Request
```

### Learning Outcome

Understand how middleware is used to protect backend APIs and validate user access.

---

# Models Folder

The models folder contains MongoDB schemas and models created using Mongoose.

---

## usermodel.js

### User Database Model

Defines the structure of user data stored in MongoDB.

### Features

- User Schema
- Field Validation
- Collection Structure
- User Data Management

### Example

```javascript
const UserSchema = new mongoose.Schema({
    name: String,
    email: String
});
```

### Learning Outcome

Learn how MongoDB schemas and collections are created using Mongoose.

---

## productmodel.js

### Product Database Model

Defines the structure of product data stored in MongoDB.

### Features

- Product Schema
- Product Validation
- Database Structure
- Collection Management

### Learning Outcome

Understand how product collections are managed within MongoDB.

---

# API Testing

## req.http

Used for testing backend APIs directly without frontend integration.

### Features

- Test GET Requests
- Test POST Requests
- Test PUT Requests
- Test DELETE Requests
- Verify API Responses
- Backend Debugging

### HTTP Methods Covered

- GET
- POST
- PUT
- DELETE

### Learning Outcome

Understand how backend APIs are tested during development.

---

# Configuration Files

## package.json

Manages project configuration, dependencies, and scripts.

### Features

- Dependency Management
- Script Configuration
- Project Metadata

### Example

```json
{
  "scripts": {
    "start": "node server.js"
  }
}
```

---

## package-lock.json

Stores exact dependency versions used in the project.

### Benefits

- Consistent Installations
- Faster npm Installs
- Stable Project Setup

---

## .gitignore

Prevents unnecessary files from being uploaded to GitHub.

### Common Ignored Files

```text
node_modules/
.env
```

---

# Core Backend Concepts Learned

## Node.js

- Runtime Environment
- Server-Side JavaScript
- Backend Execution

## Express.js

- Routing
- Middleware
- API Handling
- Server Management

## MongoDB & Mongoose

- Schemas
- Models
- Collections
- Data Validation

## Authentication

- Token Verification
- Route Protection
- Middleware Security

## REST APIs

- GET Requests
- POST Requests
- PUT Requests
- DELETE Requests

---

# Complete Backend Architecture

```text
Frontend
   ↓
HTTP Request
   ↓
Express Server
   ↓
Middleware
   ↓
API Route
   ↓
MongoDB Database
   ↓
Response
   ↓
Frontend
```

---

# Installation

Install project dependencies:

```bash
npm install
```

---

# Running the Project

Start the backend server:

```bash
node server.js
```

OR

```bash
npm start
```

---

# Skills Developed

By completing ATP WEEK-5, the following skills are developed:

- Backend Development
- Express.js API Development
- MongoDB Integration
- Mongoose Modeling
- Authentication Middleware
- REST API Architecture
- Modular Backend Design
- Database Management

---

# Future Improvements

The project can be extended with:

- JWT Authentication
- Password Encryption
- Environment Variables
- Advanced Error Handling
- CRUD Operations
- API Validation
- Deployment
- Role-Based Authorization

---

# Learning Progression

```text
Basic Backend
       ↓
REST APIs
       ↓
Database Integration
       ↓
Authentication
       ↓
Advanced Backend Architecture
```

---

# Summary

This repository represents the transition from basic backend development to advanced backend architecture using Node.js, Express.js, MongoDB, and Mongoose.

It provides a strong foundation for building scalable backend systems and full-stack web applications with authentication, database integration, and modular project structure.

---

