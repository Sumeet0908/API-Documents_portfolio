# GET User by ID
## Description
The Get User by ID API retrieves the details of a specific user registered in the system using the peovided ID.
## Endpoint
`GET /api/v1/Users/{id}`
## Path Parameters
| Parameter | Type | Required | Description |
|----------|------|----------|-------------|
| id | integer | Yes | Unique identifier used to retrieve a specific user |
## Request Body
None.
## Success Response
If the request is successful, the API returns the details of single user, including the user ID and username.
**Status Code:** `200 OK`
```json
{
    "id": 1,
    "userName": "john_doe"
}
```
## Error Response
If specific user does not exists, the API returns a not found error. **Status Code:** `404 Not Found`
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