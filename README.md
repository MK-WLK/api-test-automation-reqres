# API Test Automation: ReqRes

A hands-on API testing project created to practice API test automation using Postman and Newman.

## Overview

This project is my introduction to API test automation and CI/CD.

After spending roughly two years away from programming, I used this project to rebuild my programming fundamentals while learning API testing, JavaScript assertions, Postman, Newman, Git, and GitHub Actions.

The project was developed with assistance from AI tools, primarily OpenAI's GPT-5.6 Luna and Anthropic Claude Sonnet 5.0. AI was used to explain unfamiliar programming concepts, troubleshoot issues, and guide implementation.

This repository documents my learning process and first practical API automation project.

## API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/api/users?page=2` | Get users list |
| GET | `/api/users/2` | Get a single user |
| POST | `/api/users` | Create a user |
| PUT | `/api/users/2` | Update a user |
| DELETE | `/api/users/2` | Delete a user |

## Test Coverage

**5 API requests · 15 automated assertions**

Tests cover:

- HTTP status codes
- Response fields and data
- Created and updated user values
- Empty DELETE response
- Response time

## Test Results

**15/15 assertions passed** in the Postman Collection Runner before the ReqRes anonymous API request limit was reached.

- Requests: 5
- Assertions: 15
- Passed: 15
- Failed: 0
- Errors: 0

> **Note:** The ReqRes demo API is rate-limited for anonymous requests. Subsequent executions may return HTTP 429 (`rate_limit_exceeded`) after the limit is exhausted.

## Tools

Postman · JavaScript · Newman · Git · GitHub · GitHub Actions

## Running the Tests

### Postman

Import `collection.json` and run the collection using the Collection Runner.

### Newman

```bash
newman run collection.json