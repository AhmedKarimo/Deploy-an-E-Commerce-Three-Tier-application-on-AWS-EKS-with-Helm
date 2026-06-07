#  RobotShop EKS DevOps Project

## Overview
This project deploys a microservices-based e-commerce application (RobotShop) on AWS EKS using Kubernetes, Helm, and AWS Load Balancer Controller.

---

## Architecture
- AWS EKS (Kubernetes Cluster)
- Helm for deployment
- AWS ALB Ingress Controller
- 3-Tier Microservices Architecture:
  - Frontend (Web)
  - Backend Services (Cart, User, Payment, etc.)
  - Database (MongoDB, MySQL, Redis)

---

## Tech Stack
- AWS EKS
- Kubernetes
- Helm
- AWS IAM & IRSA
- AWS ALB (Application Load Balancer)
- Docker Containers

---


##  Screenshots

###  Application Running

<img width="1859" height="856" alt="Screenshot from 2026-06-08 01-37-23" src="https://github.com/user-attachments/assets/0dd5c9c0-cbc2-46dc-b264-6d14d44466c1" />

###  Kubernetes Pods

<img width="1352" height="394" alt="Screenshot from 2026-06-08 01-38-06" src="https://github.com/user-attachments/assets/313696bf-f208-45e2-b59a-7c9dea59650f" />


###  AWS EKS Cluster

<img width="1838" height="934" alt="Screenshot from 2026-06-08 01-38-36" src="https://github.com/user-attachments/assets/666be9f0-c370-4b12-a1f5-97cc56a074d4" />


##  Deployment Steps

```bash
eksctl create cluster ...
helm install robot-shop ...
kubectl apply -f ingress.yaml
