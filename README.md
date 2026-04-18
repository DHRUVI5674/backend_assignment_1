# 📝 Notes Management REST API

A clean and structured **RESTful API** built using **Node.js, Express, MongoDB, and Mongoose** to manage notes efficiently. This project demonstrates core backend fundamentals including CRUD operations, proper HTTP methods, MVC architecture, and data validation.

---

## 🚀 Live Demo

* 🌐 **Deployed API (Render):** https://backend-assignment-1-h4k1.onrender.com
* 📬 **Postman Documentation:** https://documenter.getpostman.com/view/50840875/2sBXqCRQgq

---

## 📌 Features

* Create a single note
* Create multiple notes (bulk insert)
* Retrieve all notes
* Retrieve a note by ID
* Replace a note completely (PUT)
* Update specific fields (PATCH)
* Delete a single note
* Delete multiple notes (bulk delete)

---

## 🛠️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB
* **ODM:** Mongoose
* **Environment Management:** dotenv
* **Development Tool:** Nodemon

---

## 📡 API Endpoints

### 🔹 Create Note

**POST** `/api/notes/notes`

### 🔹 Create Multiple Notes

**POST** `/api/notes/multiple`

### 🔹 Get All Notes

**GET** `/api/notes`

### 🔹 Get Note by ID

**GET** `/api/notes/:id`

### 🔹 Replace Note (Full Update)

**PUT** `/api/notes/:id`

### 🔹 Update Note (Partial)

**PATCH** `/api/notes/:id`

### 🔹 Delete Note

**DELETE** `/api/notes/:id`

### 🔹 Delete Multiple Notes

**DELETE** `/api/notes/multiple`

---

## ⚙️ Environment Variables

Create a `.env` file and add:

```
MONGO_URI=your_mongodb_connection_string
PORT=5000
```

---

## ▶️ Run Locally

```bash
npm install
npm run dev
```

---

## 📦 Response Format

All API responses follow a consistent structure:

```json
{
  "success": true,
  "message": "Description of the result",
  "data": {}
}
```

---

## 📊 HTTP Status Codes

* **200** – Successful GET, PUT, PATCH, DELETE
* **201** – Resource created successfully
* **400** – Bad request / validation error
* **404** – Resource not found
* **500** – Internal server error

---

## 🔍 Key Concepts Implemented

* REST API design principles
* MVC architecture
* MongoDB schema design with validation
* Proper use of HTTP methods (POST, GET, PUT, PATCH, DELETE)
* Difference between PUT and PATCH
* Bulk operations using `insertMany()` and `$in` operator
* Centralized error handling and consistent responses

---

## 🧪 Testing

All endpoints are tested using **Postman**.
You can access the full API collection here:

👉 https://documenter.getpostman.com/view/50840875/2sBXqCRQgq

---

## 🌍 Deployment

The backend is deployed on **Render** and is publicly accessible:

👉 https://backend-assignment-1-h4k1.onrender.com

---

## 📌 Final Note

This project focuses on building a strong foundation in backend development by implementing real-world REST API practices. It covers all essential operations and design principles required for modern web applications.

---
