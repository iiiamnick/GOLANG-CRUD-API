# GOLANG-CRUD-API

A simple CRUD (Create, Read, Update, Delete) REST API built with Go.
This project demonstrates how to create a basic backend service using Go’s net/http package and standard libraries.

---

## Features

* RESTful API using Go’s `net/http`
* CRUD operations (Create, Read, Update, Delete)
* JSON-based request and response handling
* Easy to extend and integrate with databases (MySQL, PostgreSQL, SQLite, etc.)
* Clean and modular structure

---

## Project Structure

```
GOLANG-CRUD-API/
│
├── handlers/         # Request handlers / controllers
├── models/           # Data models / structs
├── repository/       # Database logic (CRUD operations)
├── routes/           # API route definitions
│
├── main.go           # Application entry point
├── go.mod            # Go module definition
└── go.sum
```

---

##  Setup & Run

1. Clone the repository:

   ```bash
   git clone https://github.com/iiiamnick/GOLANG-CRUD-API.git
   cd GOLANG-CRUD-API
   ```

2. Download dependencies:

   ```bash
   go mod tidy
   ```

3. Run the application:

   ```bash
   go run main.go
   ```

4. By default, the server runs on:

   ```
   http://localhost:8080
   ```

---

## Example Endpoints

| Method | Endpoint      | Description       |
| ------ | ------------- | ----------------- |
| GET    | `/items`      | Get all items     |
| GET    | `/items/{id}` | Get a single item |
| POST   | `/items`      | Create a new item |
| PUT    | `/items/{id}` | Update an item    |
| DELETE | `/items/{id}` | Delete an item    |

---

## Example Request

**POST /items**

```json
{
  "name": "Laptop",
  "price": 75000
}
```

**Response:**

```json
{
  "id": 1,
  "name": "Laptop",
  "price": 75000
}
```

---

## Tech Stack

* **Language:** Go 1.22+
* **Libraries:** net/http, encoding/json
* **Optional:** gorilla/mux for routing 

---

##  About

This project is a learning example for Go developers exploring REST API design, routing, and modular code structure.
