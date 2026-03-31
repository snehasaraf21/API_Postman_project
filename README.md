[![Run Postman API Tests](https://github.com/snehasaraf21/API_Postman_project/actions/workflows/newman-tests.yml/badge.svg)](https://github.com/snehasaraf21/API_Postman_project/actions/workflows/newman-tests.yml)
# Restful Booker API Testing Project

This project contains API testing for the **Restful Booker API**, focusing on validating authentication, booking creation, retrieval, update, partial update, and deletion functionality using Postman.

The goal of this project is to demonstrate **API testing skills**, including request validation, negative testing, authentication handling, and response verification.

---

# Project Overview

The **Restful Booker API** is a sample REST API used for practicing API testing.  
This project validates all major API endpoints using **Postman collections, test cases, and documentation**.

---

# Tested API Endpoints

## Authentication
| Method | Endpoint | Description |
|------|------|------|
| POST | /auth | Generate authentication token |

## Booking
| Method | Endpoint | Description |
|------|------|------|
| GET | /booking | Retrieve all booking IDs |
| GET | /booking/{id} | Retrieve booking details |
| POST | /booking | Create booking |
| PUT | /booking/{id} | Update booking |
| PATCH | /booking/{id} | Partial update booking |
| DELETE | /booking/{id} | Delete booking |

## Health Check
| Method | Endpoint |
|------|------|
| GET | /ping |

---

# Tools Used

- Postman (API Testing)
- Newman (Optional for CLI execution)
- GitHub (Project hosting)
- Excel (Test case documentation)

---

**Advanced Validation: JSON Schema
Unlike basic assertions, this suite uses JSON Schema (AJV) to perform contract testing.

Data Integrity: Ensures totalprice is always a number.

Mandatory Fields: Verifies that bookingdates (checkin/checkout) are never missing.

Type Safety: Prevents null values in critical fields like lastname.
