# Concurrent Ticket Reservation System

A backend ticket reservation system built using Node.js, Express, and Redis.  
This project demonstrates how Redis can be used to handle concurrent booking requests efficiently and prevent overbooking.

---

## 🚀 Features

- Real-time seat availability management
- Prevents double booking using Redis
- REST API based backend
- Docker support for containerized deployment
- Production-ready configuration (PORT from environment variable)

---

## 🛠 Tech Stack

- Node.js
- Express.js
- Redis
- Docker

---

## 📌 API Endpoints

### 1️⃣ Check Server Status
GET /status  

Returns server health and availability status.

---

### 2️⃣ Book a Ticket
POST /book  

Books a ticket if seats are available.

---

## ⚙️ How It Works

- Redis stores the available seat count.
- When a booking request is made, Redis ensures atomic operations.
- This prevents race conditions during multiple simultaneous bookings.

---

## 🐳 Running with Docker

```bash
docker-compose up --build
```

---

## 🌍 Deployment

This project can be deployed on platforms like:

- Railway
- Render

Make sure to configure the following environment variables:

PORT  
REDIS_URL 

## Live Deployment

https://exp-43.onrender.com

---

## 📚 Learning Outcome

This project helped in understanding:

- Backend API development
- Redis integration
- Concurrency handling
- Deployment of Node.js applications
