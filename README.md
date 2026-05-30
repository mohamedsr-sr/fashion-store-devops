# 🚀 Fashion Store DevOps Project

## 🏷️ Tech Stack

![Node.js](https://img.shields.io/badge/Node.js-18.x-green?style=for-the-badge&logo=node.js)
![Express](https://img.shields.io/badge/Express.js-Backend-black?style=for-the-badge&logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?style=for-the-badge&logo=mongodb)
![Docker](https://img.shields.io/badge/Docker-Container-blue?style=for-the-badge&logo=docker)
![Microservices](https://img.shields.io/badge/Microservices-Architecture-purple?style=for-the-badge)
![REST API](https://img.shields.io/badge/REST-API-orange?style=for-the-badge)
![DevOps](https://img.shields.io/badge/DevOps-Practices-red?style=for-the-badge)
![Git](https://img.shields.io/badge/Git-Version_Control-orange?style=for-the-badge&logo=git)
![GitHub](https://img.shields.io/badge/GitHub-Repo-black?style=for-the-badge&logo=github)

---

## 📌 Overview

Fashion Store DevOps Project is a scalable backend application designed for an online fashion store. The project follows modern backend development and DevOps practices using Node.js, Express.js, MongoDB, Docker, and RESTful APIs.

The goal of this project is to simulate a real-world e-commerce platform architecture while applying DevOps concepts such as containerization, automation, scalability, and infrastructure management.

---

## 🎯 Project Objectives

* Build a scalable backend architecture
* Manage product data using MongoDB
* Create RESTful APIs for product management
* Apply Docker containerization concepts
* Prepare the application for Kubernetes deployment
* Implement CI/CD pipelines
* Add monitoring and observability tools

---

## 🏗️ Architecture

Fashion Store follows a microservice-oriented approach.

### Current Architecture:

Client  
|  
v  
Product Service (Node.js + Express)  
|  
v  
MongoDB  

---

### Future Architecture:

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

## ⚙️ Features Implemented

### 📦 Product Service

The Product Service provides APIs for managing products.

### Implemented Features:

* Create Product  
* Retrieve Products  
* MongoDB Integration  
* Environment Variables Management  
* Dockerized Database  

---

## 🧾 Product Model

Each product contains:

* Name  
* Description  
* Price  
* Image URL  
* Category  
* Stock Quantity  
* Created Date  
* Updated Date  

---

### 📌 Example:

```json
{
"name": "Black T-Shirt",
"description": "Premium cotton t-shirt",
"price": 299,
"image": "https://example.com/image.jpg",
"category": "Men",
"stock": 25
}
