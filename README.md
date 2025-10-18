### Build a Dynamic Profile Endpoint

The task requires creating a RESTful API endpoint (`/me`) that returns my profile information along with a **random cat fact** fetched dynamically from the [Cat Facts API](https://catfact.ninja/fact).

## Task Overview

The API should:

1. Expose a **GET** endpoint at `/me`.
2. Return data in **JSON** format (`Content-Type: application/json`).
3. Include:
   - My profile information (email, name, and stack)
   - The **current UTC timestamp** in ISO 8601 format
   - A **random cat fact** fetched from the Cat Facts API

## Technologies Used

- **Node.js** — JavaScript runtime
- **Express.js** — Web framework for building REST APIs
- **Axios** — For making HTTP requests to external APIs
- **CORS** — To handle cross-origin requests
- **Railway** — For hosting and deployment

## Endpoint Specification

### **GET** `/me`

**Response Structure:**

```json
{
  "status": "success",
  "user": {
    "email": "jessicaakhilome@example.com",
    "name": "Jessica Akhilome",
    "stack": "Node.js/Express"
  },
  "timestamp": "2025-10-17T12:34:56.789Z",
  "fact": "Cats have five toes on their front paws, but only four toes on their back paws."
}
```
