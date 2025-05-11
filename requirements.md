# Airbnb Clone - Technical Requirements Specification

## Table of Contents

1. [User Authentication](#user-authentication)
2. [Property Management](#property-management)
3. [Booking System](#booking-system)

---

## User Authentication

### Functional Requirements

- Secure JWT-based authentication
- Role-based access control (Guest, Host, Admin)
- OAuth 2.0 integration (Google, Facebook)
- Password recovery flow

### Technical Specifications

#### API Endpoints

| Method | Endpoint             | Description            |
| ------ | -------------------- | ---------------------- |
| POST   | `/api/auth/register` | Register new user      |
| POST   | `/api/auth/login`    | Login with credentials |
| POST   | `/api/auth/oauth`    | OAuth authentication   |
| POST   | `/api/auth/refresh`  | Refresh JWT token      |

#### Request/Response Examples

**Registration Request:**

```json
{
  "email": "user@example.com",
  "password": "SecurePass123!",
  "role": "host",
  "name": "John Doe"
}
```
