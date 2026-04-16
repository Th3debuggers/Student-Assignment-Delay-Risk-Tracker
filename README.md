“Track. Predict. Prevent.
Your assignments, always on time.”

# Student Assignment Delay & Risk Tracker

# About

This project is a web-based system that tracks assignment progress and predicts delay risk using an asynchronous, event-driven approach.

# Features

* Assignment tracking with deadlines
* Delay and risk prediction (Low / Medium / High)
* Asynchronous processing using queue
* Parallel execution using multiple workers

---

# Architecture

* Frontend sends data to backend (FastAPI)
* Backend pushes tasks to **RabbitMQ queue**
* Worker processes tasks asynchronously
* Backend returns result via API

---

## Tech Stack

* Frontend: HTML
* Backend: Python (FastAPI)
* Queue: RabbitMQ
* Worker: Python
* Database: SQLite

---

## Scalability

* Event-driven architecture
* Queue-based task handling
* Multiple workers for parallel processing
* Idempotent result updates

---

## Docker

* Backend, worker, and RabbitMQ defined in `docker-compose.yml`
* Runs in a single Docker network

---

# Usage

1. Submit assignment details
2. Backend sends task to queue
3. Worker processes risk
4. Check result using task ID

---

# Future Scope

* Notification system
* Machine learning-based prediction
* Multi-user support

