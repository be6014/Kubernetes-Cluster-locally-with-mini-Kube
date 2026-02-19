# Kubernetes Minikube Task 5

## Objective
Deploy and manage an app in Kubernetes using Minikube.

## Steps
```bash
# Start Minikube
minikube start

# Deploy app
kubectl apply -f deployment.yaml

# Expose service
kubectl apply -f service.yaml

# Verify
kubectl get pods
kubectl get svc

# Scale deployment
kubectl scale deployment nginx-deployment --replicas=4

# Describe for logs
kubectl describe pod <pod-name>
```

## Files
- deployment.yaml → Kubernetes Deployment
- service.yaml → NodePort Service
- screenshots → kubectl outputs

## Access App
minikube service nginx-service
