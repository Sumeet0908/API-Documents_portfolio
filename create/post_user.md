# Create User
## Description
Create a new user.
## Endpoint
`POST /users`
## Request Body
The request body contains name and email in JSON format. 
```json
{
    "name": "Test User",
    "email": "test@example.com",
}
```
## Response
The API Returns a user object representing the submitted data along with a generated ID in JSON format with **Status Code:** `201 Created`
```json
{
    "name": "Test User",
    "email": "test@example.com",
    "id": 11
}
```
> **Source:**
> This API is part of the public dummy REST API provided by [JSONPlaceholder](https://jsonplaceholder.typicode.com).
>## Practice Notes
> - This documentation is created as part of progressive learning in API documentation.
> - This endpoint is used to understand POST requests and request body handling.
> - The API simulates user creation and does not persist data.
> - Error responses and validations are intentionally not documented here, as they were not observed or validated during testing.
> - Documentation standards are being improved incrementally as part of daily practice.