# ATP WEEK-3 & WEEK-4: Backend Development with Node.js & Express.js

## Overview

This repository contains backend development practice projects built using **Node.js** and **Express.js**. The project demonstrates how backend servers are created, how APIs are structured, and how client-server communication works in modern web applications.

The repository focuses on building REST APIs, handling HTTP requests, organizing routes, and implementing modular backend architecture.

---

## Technologies Used

### Backend Technologies
- Node.js
- Express.js

### Development Tools
- Visual Studio Code
- Git & GitHub
- npm
- REST Client / Postman

---

## Project Structure

```text
ATP WEEK-3&4/
│
├── APIs/
│   ├── productapi.js
│   └── userapi.js
│
├── package.json
├── package-lock.json
├── req.HTTP
├── server.js
└── .gitignore
```

---

## server.js

The main entry point of the backend application.

### Responsibilities

- Create Express Server
- Configure Middleware
- Connect API Routes
- Handle Incoming Requests
- Start Backend Server
- Manage Route Registration

---

## APIs Folder

### userapi.js

Handles user-related backend operations.

Features:

- Create User
- Read User Data
- Process User Requests
- Send API Responses

### productapi.js

Handles product-related backend operations.

Features:

- Product APIs
- Product Data Processing
- Route Management
- API Responses

---

## req.HTTP

Used for testing backend APIs without frontend integration.

### Supported Methods

- GET
- POST
- PUT
- DELETE

---

## package.json

Manages:

- Project Metadata
- Dependencies
- npm Scripts

Example:

```json
{
  "scripts": {
    "start": "node server.js"
  }
}
```

---

## package-lock.json

Stores exact dependency versions to ensure consistent installations.

---

## .gitignore

Common ignored files:

```text
node_modules/
.env
```

---

## Backend Request Lifecycle

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
Business Logic
   ↓
Response
   ↓
Frontend
```

---

## Installation

```bash
npm install
```

---

## Running the Project

```bash
node server.js
```

OR

```bash
npm start
```

---

## Skills Developed

- Backend Development Fundamentals
- Node.js Application Development
- Express.js Server Creation
- API Development
- Route Handling
- Middleware Usage
- REST API Design
- API Testing
- Modular Project Architecture
- Client-Server Communication

---

## Future Improvements

- MongoDB Integration
- CRUD Operations
- Authentication
- JWT Authorization
- Environment Variables
- Input Validation
- Error Handling Middleware

---
