# 🛒 OnlineStoreAPI

API Testing Project covering **Products**, **Cart**, and **User** modules with functional and data-driven validation.

---

## 📌 Project Overview

This project demonstrates end-to-end API testing using:

- Postman (Collections & Environments)
- Newman (CLI execution & reporting)
- CI/CD (Jenkins / GitHub Actions)

The APIs support full **CRUD operations**, filtering, sorting, authentication, and error handling.

---

## 📦 Modules

### 1️⃣ Products

- GET `/products`
- GET `/products/{id}`
- GET `/products?limit=`
- GET `/products?sort=`
- GET `/products/categories`
- GET `/products/category/{category}`
- POST `/products`
- PUT `/products/{id}`
- PATCH `/products/{id}`
- DELETE `/products/{id}`

---

### 2️⃣ Cart

- GET `/carts`
- GET `/carts/{id}`
- GET `/carts?limit=`
- GET `/carts?sort=`
- GET `/carts?startDate=&endDate=`
- GET `/carts/user/{userId}`
- POST `/carts`
- PUT `/carts/{id}`
- PATCH `/carts/{id}`
- DELETE `/carts/{id}`

---

### 3️⃣ User

- POST `/auth/login`
- GET `/users`
- GET `/users/{id}`
- POST `/users`
- PUT `/users/{id}`
- PATCH `/users/{id}`

---

## 🧪 Testing Approach

- Test cases created from technical documentation and stakeholder discussions
- No hardcoded data (all values managed through variables)
- Data-driven testing:
  - JSON → Single execution cycle
  - CSV → Multiple datasets

Supported Test Management Tools:
- TestRail
- JIRA (Zephyr / Xray)
- Azure DevOps
- qTest
- TestLink

---

## ▶️ Running with Newman

Postman does not provide detailed reports by default.

Run collection using Newman:

```bash
newman run collection.json -e environment.json -r html
