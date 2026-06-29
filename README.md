# Azure DevOps Microservices App Kubernetes Deployment

## 📌 Project Overview

This project demonstrates a complete CI/CD pipeline for deploying a cloud-native microservices application using **Azure DevOps** and **Kubernetes**.

The application consists of multiple independent microservices that are automatically built, tested, containerized, and deployed to **Test** and **Production** Kubernetes clusters through Azure DevOps Pipelines.

---

## 🚀 Tech Stack

* Azure DevOps
* Azure Repos
* Azure Pipelines
* Docker
* Kubernetes (K8s)
* YAML Pipelines
* Microservices Architecture
* Redis

---

## 🏗️ Project Architecture

The application is composed of the following microservices:

| Service               | Description                          |
| --------------------- | ------------------------------------ |
| frontend              | Web application frontend             |
| productcatalogservice | Provides product catalog information |
| recommendationservice | Generates product recommendations    |
| cartservice           | Handles shopping cart operations     |
| redis-cart            | Redis database for cart storage      |
| checkoutservice       | Processes customer checkout          |
| paymentservice        | Handles payment transactions         |
| shippingservice       | Manages shipping operations          |
| currencyservice       | Currency conversion service          |
| emailservice          | Sends order confirmation emails      |
| adservice             | Displays advertisements              |
| loadgenerator         | Generates simulated user traffic     |


<img width="3556" height="1954" alt="image" src="https://github.com/user-attachments/assets/b898abd7-548c-4076-8333-596d339c643c" />
---

---

## ⚙️ CI/CD Pipeline

The Azure DevOps pipeline performs the following stages:

### Continuous Integration (CI)

* Pull source code from Azure Repos
* Restore dependencies
* Build all microservices
* Run automated tests
* Build Docker images
* Push Docker images to Docker Hub

### Continuous Deployment (CD)

Deploys automatically to:

* ✅ Test Kubernetes Cluster
* ✅ Production Kubernetes Cluster

Deployment is performed using Kubernetes YAML manifests.

---

## ☸️ Kubernetes Deployment

Currently deployed services:

```
frontend
productcatalogservice
recommendationservice
cartservice
redis-cart
checkoutservice
paymentservice
shippingservice
currencyservice
emailservice
adservice
loadgenerator
```

Deployment Status

```
12/12 Services Running
Pods Status: Running
Restart Count: 0
```

---

## 📋 Kubernetes Pods

```
adservice
cartservice
checkoutservice
currencyservice
emailservice
frontend
loadgenerator
paymentservice
productcatalogservice
recommendationservice
redis-cart
shippingservice
```

---

## 🔄 Deployment Workflow

```
Developer
     │
     ▼
Azure Repos
     │
     ▼
Azure DevOps Pipeline
     │
     ▼
Build & Test
     │
     ▼
Docker Image Build
     │
     ▼
Docker Hub
     │
     ▼
Deploy to Test Kubernetes Cluster
     │
     ▼
Validation
     │
     ▼
Deploy to Production Kubernetes Cluster
```
<img width="1848" height="1045" alt="image" src="https://github.com/user-attachments/assets/6eaeb7f1-56bf-4e15-b2f2-363f18ddc57b" />

---


## 📊 Features

* Microservices-based architecture
* Azure DevOps CI/CD
* Docker containerization
* Kubernetes orchestration
* Automated deployments
* Separate Test and Production environments
* Infrastructure as Code using YAML
* Scalable and cloud-native deployment

---



## 📸 Sample Output

```
NAME                                     READY   STATUS    RESTARTS
adservice                               1/1     Running   0
cartservice                             1/1     Running   0
checkoutservice                         1/1     Running   0
currencyservice                         1/1     Running   0
emailservice                            1/1     Running   0
frontend                                1/1     Running   0
loadgenerator                           1/1     Running   0
paymentservice                          1/1     Running   0
productcatalogservice                   1/1     Running   0
recommendationservice                   1/1     Running   0
redis-cart                              1/1     Running   0
shippingservice                         1/1     Running   0
```
<img width="3216" height="2448" alt="online-boutique-frontend-1" src="https://github.com/user-attachments/assets/bd1bf7c0-aca3-46f4-a79d-711a45a7b580" />




## 👨‍💻 Author

**Hanzala Israr**


