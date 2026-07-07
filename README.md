# Docker Kubernetes Assignment

## Docker Images
- Version 1: tpallavipatra/exercise:1
- Version 2: tpallavipatra/exercise:2

## Docker Hub
https://hub.docker.com/r/tpallavipatra/exercise

## Kubernetes
- Deployment with 4 replicas
- NodePort Service (30080)
- Resource requests and limits
- Readiness Probe
- Liveness Probe
- Rolling Update
- Rollback to Version 1

## Commands Used

### Create Deployment
```bash
kubectl apply -f exercise-deployment.yaml
```

### Create Service
```bash
kubectl apply -f exercise-service.yaml
```

### Update Image
```bash
kubectl set image deployment/exercise exercise=tpallavipatra/exercise:2
```

### Rollback
```bash
kubectl rollout undo deployment/exercise
```
