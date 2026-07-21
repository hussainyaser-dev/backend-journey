# Understanding HTTP & HTTPS

## 🌐 What is HTTP?
- **HTTP (HyperText Transfer Protocol)** is the foundation of communication on the web.
- It defines how clients (like browsers) and servers exchange requests and responses.
- It is **stateless** → each request is independent.
- **HTTPS = HTTP + encryption (via SSL/TLS)**, which secures communication.

---

## 📊 HTTP Server Flow

### 1. HTTP Servers
- Handle incoming requests and send responses.
- Examples: Express.js, Spring Boot, Flask.

### 2. Request Methods
- **GET** → fetch data
- **POST** → send data
- **PUT/PATCH** → update data
- **DELETE** → remove data

### 3. URL Route
- Path that identifies a resource.
- Example: `/users/123` → fetch user with ID 123.

### 4. Query Params, Headers, Body
- **Query params**: extra info in URL (`?sort=asc`)
- **Headers**: metadata (auth tokens, content type)
- **Body**: actual data sent (JSON, form data)

### 5. Status Codes
- **200 OK** → success
- **404 Not Found** → resource missing
- **500 Internal Server Error** → server crash
- **401 Unauthorized / 403 Forbidden** → authentication/authorization issues

### 6. Response Types
- **HTML** → web pages
- **JSON** → APIs
- **Text** → plain responses/logs

---

## 🔒 HTTPS Workflow

1. **Client Request**
   - Browser sends request to server using HTTPS.
   - Example: `https://example.com`.

2. **DNS Resolution**
   - Domain name is translated into IP address.

3. **TCP Handshake**
   - Client and server establish a connection.

4. **TLS/SSL Handshake**
   - Server sends certificate.
   - Client verifies authenticity.
   - Both agree on encryption keys.

5. **Encrypted Communication**
   - All HTTP data (headers, body, cookies) is encrypted.
   - Prevents eavesdropping and tampering.

6. **Server Response**
   - Server sends back secure response.
   - Includes status codes and content.
