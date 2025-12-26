# Create User
## Description
The Create User API allows new users to be registered in the system by providing a user ID, username, and password. The API stores the provided user information on the server and returns a confirmation response upon successful user creatin. If the request data is invalid, an appropriate error response is returned.
## Endpoint
`POST /api/v1/Users`
## Request Body
The request body must contain the user ID, username, and password in JSON format to create a new user.
```json
{
    "id": 1,
    "username": "john_doe",
    "password": "password123"
}
```
## Success Response
If the user is created succcessfully, the API returns a success resposnse confirming that the user has been created.
**Status Code:** `200 OK`
```json
{
    "message": "User created successfully"
}
```
## Error Response
If the request contains invalid user data, such as a duplicate username or missing required fields, the API returns an error response.
**Status Code:** `400 Bad Request`
```json
{
    "error": "Invalid user data"
}
```
## Status Codes Summary
| Status Code | Description |
|------------|-------------|
| 200 | User created successfully |
| 400 | Invalid or incomplete user data |
| 500 | Internal server error |
> **API Source:**  
> This API is documented based on the [Fake REST API](https://fakerestapi.azurewebsites.net/index.html).