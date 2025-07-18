# 🚕 Spring-Boot-Kafka-Cab-App-Main

This project is a **Cab Booking Application** built using **Spring Boot** and **Apache Kafka**. It simulates a real-time cab dispatch system where ride requests and driver updates are handled through asynchronous messaging.

---

## 🚀 Features

- 📥 Book a cab (ride request)
- 📤 Real-time ride assignment via Kafka
- 🧑‍✈️ Driver location and availability updates
- 📦 Event-driven architecture
- 🔁 Producer/Consumer model with Kafka topics
- 🛠️ Scalable and decoupled service design

---

## 🛠️ Tech Stack

- **Java 17+**
- **Spring Boot**
- **Apache Kafka** (Spring for Apache Kafka)
- **Spring Data JPA**
- **PostgreSQL / MySQL**
- **Docker & Docker Compose**
- **Lombok**, **MapStruct** (optional)
- **Swagger / SpringDoc**

---

## 🧩 Architecture Overview

Client ➝ RideController ➝ Kafka Producer ➝ ride_requests topic ➝ Kafka Consumer ➝ Driver Service


- Ride booking events are pushed to Kafka
- Driver service listens and assigns rides
- Responses and status updates may also use Kafka topics (e.g., ride_status)

---

## 📂 Project Structure

Spring-Boot-kafka-cab-app-main/
├── controller/
├── dto/
├── entity/
├── kafka/
│ ├── producer/
│ └── consumer/
├── service/
├── repository/
├── config/
└── exception/
