**Flask Application for CRUD operations on MongoDB**

This project is a Flask application that performs CRUD (Create, Read, Update, Delete) operations on a MongoDB database for a User resource using a REST API.

## Table of Contents

- [Installation](#installation)
- [API Endpoints](#api-endpoints)
- [Testing with Postman](#testing-with-postman)

## Installation
1.Install mongoDB
2.Install mongo Compass
3.Install Flask
4.Install pymongo
5.Install Postman

## API Endpoints
1.GET /users: Returns a list of all users.

2.GET /users/<id>: Returns the user with the specified ID.

3.POST /users: Creates a new user with the specified data.

4.PUT /users/<id>: Updates the user with the specified ID with the new data.

5.DELETE /users/<id>: Deletes the user with the specified ID.

## Testing with Postman

1.Create a New Request:

      Method: POST
      URL: http://localhost:5000/users
      Body:
        {
          "name": "John Doe",
          "email": "john.doe@example.com",
          "pwd": "securepassword"
        }
      Click Send to create a new user.

2.Get All Users:

    Method: GET
    URL: http://localhost:5000/users
    Click Send to retrieve the list of users.
    
3.Get User by ID:

    Method: GET
    URL: http://localhost:5000/users/<id>
    Replace <id> with the actual user ID.
    Click Send to retrieve the user details.
    
4.Update User by ID:

    Method: PUT
    URL: http://localhost:5000/users/<id>
    Replace <id> with the actual user ID.
    Body:
      {
        "name": "John Doe Updated",
        "email": "john.doe.updated@example.com",
        "pwd": "newsecurepassword"
      }
    Click Send to update the user details.

5.Delete User by ID:

    Method: DELETE
    URL: http://localhost:5000/users/<id>
    Replace <id> with the actual user ID.
    Click Send to delete the user.


