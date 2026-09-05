# API Test Automation: ReqRes

A hands-on API testing project created to practice API test automation using Postman and Newman.

## Project Overview

This project is my introduction to API test automation and CI/CD.

After spending roughly two years away from programming, I used this project to relearn programming concepts while getting hands-on experience with API testing, JavaScript assertions, Postman, Newman, Git, and GitHub Actions.

The project was developed with assistance from AI tools, primarily OpenAI's GPT-5.6 Luna and Anthropic Claude Sonnet 5.0. The AI assistance was used to explain unfamiliar programming concepts, help build and troubleshoot test scripts, and guide me through the automation workflow.

Rather than presenting this as production-level automation experience, this repository documents my learning process and my first practical API automation project.

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

## Test Results

The Postman Collection Runner successfully executed all 5 requests with 15/15 assertions passing before the ReqRes anonymous API request limit was reached.

- Requests: 5
- Assertions: 15
- Passed: 15
- Failed: 0
- Errors: 0

> Note: The ReqRes demo API has a rate limit for anonymous requests. Subsequent executions may return HTTP 429 (`rate_limit_exceeded`) after the daily limit has been exhausted. These failures are caused by the external API rate limit rather than the test assertions themselves.

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

The goal of this project was to rebuild my programming fundamentals while learning the basics of software QA automation.

Through this project, I practiced:

- Understanding REST API requests and responses
- Writing JavaScript test assertions
- Structuring API tests in Postman
- Running tests with Newman from the command line
- Using Git and GitHub for version control
- Integrating automated tests into a GitHub Actions CI pipeline

This project represents an early step in my transition from manual QA toward automation testing.