# 🔌 03 - API Testing

## 📌 Overview

- API testing validates backend behavior, data exchange, and business logic.
- It is essential for modern distributed systems and integrations.

## 📦 XML & JSON Basics

Example JSON:

```json
{
  "userId": 1,
  "name": "Alice",
  "email": "alice@example.com"
}
```

Example XML:

```xml
<user>
  <id>1</id>
  <name>Alice</name>
  <email>alice@example.com</email>
</user>
```

## 🌐 API Basics

- HTTP methods:
  - GET → read data
  - POST → create data
  - PUT → update a full resource
  - PATCH → partial update
  - DELETE → remove data

Common status codes:

- 200 OK
- 201 Created
- 400 Bad Request
- 401 Unauthorized
- 403 Forbidden
- 404 Not Found
- 500 Internal Server Error

## 🔐 Authentication Methods

- Basic Auth
- Bearer Token
- API Key
- OAuth 2.0
- JWT

Example JWT usage:

```http
Authorization: Bearer <token>
```

## 🧪 REST API Concepts

- Resource-based URLs
- Stateless communication
- Standard response formats
- Versioning examples:
  - `/api/v1/users`
  - `/api/v2/users`

## 🧰 Postman Essentials

- Collections for grouping requests
- Environments for dev/test/prod
- Pre-request scripts for setup
- Test scripts for assertions

Example Postman test:

```javascript
pm.test("Status code is 200", function () {
  pm.response.to.have.status(200);
});

pm.test("Response contains userId", function () {
  var jsonData = pm.response.json();
  pm.expect(jsonData).to.have.property("userId");
});
```

## 🧠 Interview Topics

- Difference between REST and SOAP
- Idempotency
- Caching
- Pagination
- Rate limiting
- Error handling
