# Fashion Store DevOps Project

## Overview

Fashion Store DevOps Project is a scalable backend application designed for an online fashion store. The project follows modern backend development and DevOps practices using Node.js, Express.js, MongoDB, Docker, and RESTful APIs.

The goal of this project is to simulate a real-world e-commerce platform architecture while applying DevOps concepts such as containerization, automation, scalability, and infrastructure management.

---

## Project Objectives

* Build a scalable backend architecture
* Manage product data using MongoDB
* Create RESTful APIs for product management
* Apply Docker containerization concepts
* Prepare the application for Kubernetes deployment
* Implement CI/CD pipelines
* Add monitoring and observability tools

---

## Architecture

Fashion Store follows a microservice-oriented approach.

Current Architecture:

Client
|
v
Product Service (Node.js + Express)
|
v
MongoDB

Future Architecture:

Frontend (React)
|
v
Nginx Reverse Proxy
|
v
API Gateway
|
v
Product Service
|
v
MongoDB

Containerized using Docker

Managed by Kubernetes

Automated through CI/CD Pipelines

---

## Features Implemented

### Product Service

The Product Service provides APIs for managing products.

Implemented Features:

* Create Product
* Retrieve Products
* MongoDB Integration
* Environment Variables Management
* Dockerized Database

---

## Product Model

Each product contains:

* Name
* Description
* Price
* Image URL
* Category
* Stock Quantity
* Created Date
* Updated Date

Example:

{
"name": "Black T-Shirt",
"description": "Premium cotton t-shirt",
"price": 299,
"image": "https://example.com/image.jpg",
"category": "Men",
"stock": 25
}

---

## Technologies Used

### Backend

* Node.js
* Express.js

### Database

* MongoDB
* Mongoose

### DevOps

* Docker

### Version Control

* Git
* GitHub

### Testing Tools

* Thunder Client
* Postman

---

## Project Structure

fashion-store-devops/

services/
└── product-service/
├── src/
│ ├── config/
│ │ └── db.js
│ │
│ ├── models/
│ │ └── Product.js
│ │
│ ├── routes/
│ │ └── productRoutes.js
│ │
│ └── app.js
│
├── .env
├── package.json
└── package-lock.json

---

## API Endpoints

### Health Check

GET /

Response:

{
"service": "product-service",
"status": "running"
}

---

### Get All Products

GET /api/products

Response:

[
{
"_id": "...",
"name": "Black T-Shirt",
"price": 299
}
]

---

### Create Product

POST /api/products

Request Body:

{
"name": "Black T-Shirt",
"description": "Premium cotton t-shirt",
"price": 299,
"category": "Men",
"stock": 25
}

Response:

{
"_id": "...",
"name": "Black T-Shirt",
"description": "Premium cotton t-shirt",
"price": 299,
"category": "Men",
"stock": 25
}

---

## Environment Variables

Create a .env file:

PORT=5001

MONGO_URI=mongodb://localhost:27017/fashion-store

---

## Running the Project

### Install Dependencies

npm install

### Run Development Server

npm run dev

### Run Production Server

npm start

---

## Docker

MongoDB is currently running inside Docker.

Example:

docker run -d 
--name mongodb 
-p 27017:27017 
mongo

---

## Future DevOps Roadmap

The following DevOps stages will be implemented next:

### Dockerize Product Service

* Create Dockerfile
* Build Docker Images
* Run Containers

### Docker Compose

* Product Service
* MongoDB
* Networking

### Kubernetes

* Deployments
* Services
* ConfigMaps
* Secrets
* Horizontal Scaling

### CI/CD

Using GitHub Actions:

* Build
* Test
* Docker Build
* Deployment Automation

### Monitoring

* Prometheus
* Grafana
* Application Metrics
* Container Monitoring

### Logging

* Centralized Logging
* Log Aggregation
* Error Tracking

---

## Learning Outcomes

Through this project I practiced:

* Backend Development
* REST API Design
* Database Integration
* MongoDB Modeling
* Docker Fundamentals
* DevOps Foundations
* Microservices Concepts
* Environment Management
* Git Workflow

---

## Author

Mohamed Yasser

Aspiring DevOps Engineer | Cloud & Backend Enthusiast

Building real-world projects with Docker, Kubernetes, CI/CD, and Cloud Technologies.
