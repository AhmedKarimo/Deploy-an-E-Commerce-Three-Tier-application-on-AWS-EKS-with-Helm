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

##  Deployment Steps

```bash
eksctl create cluster ...
helm install robot-shop ...
kubectl apply -f ingress.yaml
