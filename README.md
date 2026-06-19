# KUBERNETES-DEPLOYMENT

##  Project Description
This project demonstrates deployment of a microservices-based application using Kubernetes.

It includes:
- Frontend (NGINX)
- Backend (Node.js service)
- Database (MongoDB)



##  Components

### Frontend
- Runs on NGINX
- Exposed using NodePort (30080)

### Backend
- Simple Node.js HTTP server
- Exposed internally using ClusterIP

### Database
- MongoDB container
- Internal Kubernetes service



##  How to Deploy

Run the following commands:

```bash
kubectl apply -f frontend-deployment.yaml
kubectl apply -f frontend-service.yaml
kubectl apply -f backend-deployment.yaml
kubectl apply -f backend-service.yaml
kubectl apply -f mongodb-deployment.yaml
kubectl apply -f mongodb-service.yaml
