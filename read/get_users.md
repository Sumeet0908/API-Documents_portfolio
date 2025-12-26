# Get Users
## Description
This API retrives a list of all users registered in the system. The API returns user details such as user ID, name, username, email, address, and company details for each user.
## Endpoint
`GET /users`
## Request Body
None.
## Query Parameters
None.
## Response
After processing the request successfully, this API returns the array of user objects in JSON format. **Status Code:** `200 OK`
```json
[
    {
        "id": 1,
        "name": "Leanne Graham",
        "username": "Bret",
        "email": "Sincere@april.biz",
        "address": {
            "street": "Kulas Light",
            "suite": "Apt. 556",
            "city": "Gwenborough",
            "zipcode": "92998-3874",
            "geo": {
                "lat": "-37.3159",
                "lng": "81.1496"
            }
        },
        "phone": "1-770-736-8031 x56442",
        "website": "hildegard.org",
        "company": {
            "name": "Romaguera-Crona",
            "catchPhrase": "Multi-layered client-server neural-net",
            "bs": "harness real-time e-markets"
        }
    },
    {
        "id": 2,
        "name": "Ervin Howell",
        "username": "Antonette",
        "email": "Shanna@melissa.tv",
        "address": {
            "street": "Victor Plains",
            "suite": "Suite 879",
            "city": "Wisokyburgh",
            "zipcode": "90566-7771",
            "geo": {
                "lat": "-43.9509",
                "lng": "-34.4618"
            }
        },
        "phone": "010-692-6593 x09125",
        "website": "anastasia.net",
        "company": {
            "name": "Deckow-Crist",
            "catchPhrase": "Proactive didactic contingency",
            "bs": "synergize scalable supply-chains"
        }
    },
]
```
> **API Source:**
> This API is part of the public dummy REST API provided by [JSONPlaceholder](https://jsonplaceholder.typicode.com).
>## Practice Notes
>This documentation is created for learning and practice purposes.
>The goal is to understand API behavior, Postman usage, and technical documentation structure.
>More endpoints and advanced details will be added incrementally as part of daily practice.