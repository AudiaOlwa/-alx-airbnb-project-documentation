# Technical & Functional Requirements

This document specifies the requirements for key backend features of the **ALX Airbnb Project**.  
It includes API endpoints, input/output specifications, validation rules, and performance criteria.

---

## 1. User Authentication

### Functional Requirements
- Users must be able to **register**, **log in**, and **log out**.
- Passwords must be **encrypted** before storage.
- Authentication should support **JWT-based sessions**.

### API Endpoints
- `POST /api/auth/register` → Create a new account
- `POST /api/auth/login` → Authenticate user & return token
- `POST /api/auth/logout` → Invalidate user session

### Input/Output Specifications
**Register Input (JSON):**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "securePass123"
}
