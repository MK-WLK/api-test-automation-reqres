# API Test Automation — ReqRes

A hands-on API testing project created to practice API test automation using Postman and Newman.

## Project Overview

This project tests the ReqRes REST API using a Postman collection with automated response assertions.

The project covers:

- API request and response validation
- HTTP status code validation
- JSON response validation
- Response data assertions
- Response time validation
- Postman Collection Runner
- Newman command-line execution
- GitHub Actions CI integration

## API Endpoints Tested

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/api/users?page=2` | Get users list |
| GET | `/api/users/2` | Get a single user |
| POST | `/api/users` | Create a user |
| PUT | `/api/users/2` | Update a user |
| DELETE | `/api/users/2` | Delete a user |

## Test Coverage

The Postman collection currently contains 15 automated assertions across 5 API requests.

### Assertions include:

- Expected HTTP status codes
- Required response fields
- User data validation
- Created user ID validation
- Updated user data validation
- Empty DELETE response validation
- Response time validation

## Tools

- Postman
- JavaScript
- Newman
- Git
- GitHub
- GitHub Actions

## Running the Tests

Import `collection.json` into Postman and run the collection using the Collection Runner.

Newman can also be used to execute the collection from the command line.

## Project Goal

This project is part of my learning journey into software QA automation, with a focus on API testing, test scripting, command-line execution, and CI/CD integration.