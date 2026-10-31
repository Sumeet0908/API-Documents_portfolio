# API Documentation Portfolio

REST API reference documentation written in Markdown. The documentation
covers user-related endpoints (create, read, update) from public demo
APIs, tested with Postman.

## Documented endpoints

| Operation | Method | Endpoint | Source | Folder |
|---|---|---|---|---|
| Read | GET | `/users` | JSONPlaceholder | [read](read/) |
| Read | GET | `/api/v1/Users` | Fake REST API | [read](read/) |
| Read | GET | `/api/v1/Users/{id}` | Fake REST API | [read](read/) |
| Create | POST | `/users` | JSONPlaceholder | [create](create/) |
| Create | POST | `/api/v1/Users` | Fake REST API | [create](create/) |
| Create | POST | `/auth/login` | Public demo API | [create](create/) |
| Update | PUT | `/users/{id}` | JSONPlaceholder | [update](update/) |
| Update | PUT | `/api/v1/Users/{id}` | Fake REST API | [update](update/) |

## What each document contains

- Description and endpoint
- Path parameters and request body (where applicable)
- Example success response
- Error responses
- Status codes

## API sources

All endpoints are from public demo REST APIs, used for learning and
practice only:

- [JSONPlaceholder](https://jsonplaceholder.typicode.com)
- [Fake REST API](https://fakerestapi.azurewebsites.net/index.html)

## Tools

- Postman for API testing
- Markdown (VS Code) for documentation
- Git and GitHub for version control

## About this repository

This repository is an active portfolio. Some documents were written
earlier and follow simpler patterns than the newer ones. Earlier versions
of every file are available in the commit history.
