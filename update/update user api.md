# Update User API
This API allows updating the details of an existing user using the user ID.
## Endpoint
PUT /users/{id}
## Path Parameters
| Parameter | Type | Required | Description |
|----------|------|----------|-------------|
| id | integer | Yes | Unique identifier of the user |
## Request Body
The request body contains the user details to be updated.
```json
{
  "name": "Updated User",
  "username": "updateduser",
  "email": "updateduser@example.com"
}
```
## Success Response
If the update request is successful, the API returns the updated user object. `Status Code: 200 OK`
```json
{
    "name": "Updated User",
    "username": "updateduser",
    "email": "updateduser@example.com",
    "id": 1
}
```
## Error Handling
### User Not Found
If the specified user ID does not exist, the API returns an error response.
**Status Code:** `404 Not Found`
```json
{
  "error": "User not found"
}
```
### Invalid Request Data
If the request body is missing required fields or contains invalid data, the API returns a bad request error. **Status Code:** `400 Bad Request`
```json
{
  "error": "Invalid request data"
}
```
### Server Error
If an unexpected server error occurs while processing the request, the API returns an internal server error.
**Status Code:** `500 Internal Server Error`
```json
{
  "error": "Internal server error"
}
```
> **API Source:**
> This API documentation is created based on the [JSONPlaceholder](https://jsonplaceholder.typicode.com/users).