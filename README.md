# REST API with Node.js, Express, and MySQL
This project is a simple REST API built using Node.js, Express, and MySQL, following the [LogRocket tutorial](https://blog.logrocket.com/build-rest-api-node-express-mysql/).
I set up the MySQL database using [Alwaysdata](https://www.alwaysdata.com/en/), usind their free tier service. 

## Overview
The REST API provides endpoints to perform CRUD (Create, Read, Update, Delete) operations on a MySQL database. It demonstrates how to:

- Set up a Node.js project with Express.js for routing.
- Configure and connect a MySQL database.
- Implement RESTful endpoints for handling API requests.
- Use Postman (or similar tools) to test API endpoints.
  
## Features
GET: Retrieve data from the database.
POST: Add new records to the database.
PUT: Update existing records in the database.
DELETE: Remove records from the database.

## Project Structure

```bash
project-root/
├── node_modules/     # Dependencies
├── src/
│   ├── controllers/  # Logic for handling API requests
│   ├── routes/       # API routes
│   ├── config/       # Database configuration
│   └── app.js        # Main application file
├── package.json      # Project metadata and dependencies
├── .env              # Environment variables (e.g., DB credentials)
└── README.md         # Project documentation
```

## How to Run

Clone the repository:
```bash
git clone <repository-url>
cd <repository-folder>
```

Install dependencies:
```bash
npm install
```

Set up environment variables: Create a .env file in the root directory with the following contents:
```bash
DB_HOST=your-database-host
DB_USER=your-database-username
DB_PASSWORD=your-database-password
DB_NAME=your-database-name
```
Run the server:
```bash
npm start
The server will start at http://localhost:3000 (or your configured port)
```
Test the API: Use Postman or a similar tool to test the endpoints:

```bash
GET /api/resource
POST /api/resource
PUT /api/resource/:id
DELETE /api/resource/:id
```

### Technologies Used:
- Node.js
- Express.js
- MySQL
- dotenv (for environment variables)

## Future Enhancements
- Add user authentication (e.g., JWT).
- Implement validation middleware for request data.
- Extend API functionality with additional endpoints.
- Use an ORM like Sequelize for database interactions.
