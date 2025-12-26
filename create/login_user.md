# Public Login
## Description
The Login API authenticates user using their username and password.
## Endpoint
`POST /auth/login`
## Request Body
The request body contains the username and password in JSON format
```json
{
    "username": "mor_2314",
    "password": "83r5^_"
}
```
## Success Response
Returns 200 OK with an access token on successful authentication.
```json
{
    "message": "Login successful",
    "token": "jwt_token_here"
}
```
## Error Response
Returns 401 Unauthorized if authentication fails.
```json
{
    "error": "Invalid username or password"
}