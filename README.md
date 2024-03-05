
# HCM(Human Capital Management) API using Fiber Framework in GO

This repository has an API implementation for a Human Resource Management System (HRMS) using the Fiber web framework in Go. The API provides CRUD (Create, Read, Update, Delete) operations for managing employee records stored in a MongoDB database.

## Endpoints

The following endpoints are available:

- `GET /employee`: Retrieves all employee records.
- `POST /employee`: Creates a new employee record.
- `PUT /employee/:id`: Updates an existing employee record by ID.
- `DELETE /employee/:id`: Deletes an employee record by ID.

## Data Model

The `Employee` struct represents an employee record with the following fields:

- `ID` (auto-generated): The unique identifier for the employee.
- `Name`: The name of the employee.
- `Salary`: The salary of the employee.
- `Age`: The age of the employee.

## Usage

To use the HRMS API, you can use tools like cURL or Postman to send HTTP requests to the defined endpoints.

Here are some examples:

- Retrieve all employee records:
  ```
  GET http://localhost:3000/employee
  ```

- Create a new employee record:
  ```
  POST http://localhost:3000/employee
  Content-Type: application/json

  {
    "name": "John Doe",
    "salary": 5000,
    "age": 30
  }
  ```

- Update an employee record by ID:
  ```
  PUT http://localhost:3000/employee/{id}
  Content-Type: application/json

  {
    "name": "Updated Name",
    "salary": 6000,
    "age": 35
  }
  ```

- Delete an employee record by ID:
  ```
  DELETE http://localhost:3000/employee/{id}
  ```

Feel free to explore and test the API using different HTTP methods and data.

## Conclusion

The Fiber HCM API provides a basic implementation for managing employee records. It demonstrates the usage of the Fiber web framework and integration with MongoDB. You can further extend and customize the API based on your HCM requirements or integrate it into larger systems.
