# GET All User
## Description
The Get All Users API retrives a list of all users registered in the system. The API returns user details such as user ID and username for each user.
## Endpoint
`GET /api/v1/Users`
## Request Body
None.
## Success Responsse
If the request is successful, the API returns a list of all user along with their user ID and username. **Status Code:** `200 OK`
```json
[
    {
        "id": 1,
        "username": "john_doe"
    },
    {
        "id": 2,
        "username": "jane_smith"
    }
]
```
## Error Response
If an unexpected server issue occurs while processing the request, the API returns an error response. **Status Code:** `500 Internal Server Error`
```json
{
    "error": "Internal Server Error"
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