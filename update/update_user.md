# Update User
## Description
The Update User API allows updating the details of an existing user using the provided user ID. The API accepts new data and updates the corresponding user records in the system.
## Endpoint
`PUT /api/v1/Users/{id}`
## Path Parameters
| Parameter | Type | Required | Description |
|----------|------|----------|-------------|
| id | integer | Yes | Unique identifier of the user to be updated |
## Request Body
The request body contains the updated user details in JSON format for the specified user.
```json
{
    "userName": "Alex_Peter",
    "Password": "Alex@123"
}
```
## Success Responsse
If the update request is successful, the API confirms the update and returns a success message. **Status Code:** `200 OK`
```json
{
    "message": "User updated successfully"
}
```
## Error Response
If specified user does not exists, the API returns a not found error. **Status Code:** `404 Not Found`
```json
{
    "error": "User not found"
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