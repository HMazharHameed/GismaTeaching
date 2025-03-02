# Task: Create a Spring Boot REST API with Database Interaction  

## Objective  
Build a Spring Boot REST API that connects to a database, allowing users to store and retrieve data.  

##  Instructions  

###  Step 1: Create an Entity  
- Define a User entity with `id`, `name`, and `email` fields.  
- Use JPA annotations to map it to a database table.  

### Step 2: Create a Repository  
- Implement a JPA repository for managing database operations.  
- Extend the correct interface to provide CRUD functionality.  

### Step 3: Create a REST Controller  
- Implement an API endpoint to fetch all users from the database.  
- Implement an API endpoint to add a new user to the database.  
- Use proper HTTP methods (`GET`, `POST`) for each operation.  

### Step 4: Configure the Database  
- Use any database image for testing.  
- Define database connection properties in **application.properties**.  

### Step 5: Run the Application  
- Start the Spring Boot application.  
- Ensure the API is running on the default port (`8080`).  

### Step 6: Test the API  
- Retrieve all users by making a `GET` request to `/api/users`.  
- Add a new user by sending a `POST` request with `name` and `email` in the request body.  
- Verify that the data is stored and retrieved correctly.  
