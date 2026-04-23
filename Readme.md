## Kubernetes Day 1 - Introduction

- Learned what Kubernetes is
- Understood container orchestration
- Compared Docker vs Kubernetes
- Installed Minikube (local Kubernetes cluster)
- Ran first kubectl command

### Commands Used
- minikube start
- kubectl get nodes

## Kubernetes Day 2 - Pods

- Learned what a Pod is in Kubernetes
- Created first Pod using YAML configuration
- Ran container inside Kubernetes
- Used kubectl commands to manage Pods
- Accessed Pod using port-forward

### Commands Used
- kubectl apply -f pod.yaml
- kubectl get pods
- kubectl describe pod
- kubectl logs
- kubectl port-forward
- kubectl delete -f pod.yaml

## Kubernetes Day 3 - Deployments

- Learned why Pods are not used directly in production
- Created Deployment to manage Pods
- Ran multiple replicas of application
- Tested auto-healing by deleting Pods
- Scaled application using kubectl

### Commands Used
- kubectl apply -f deployment.yaml
- kubectl get deployments
- kubectl get pods
- kubectl delete pod
- kubectl scale deployment
- kubectl delete -f deployment.yaml

## Kubernetes Day 4 - Services

- Learned how to expose applications in Kubernetes
- Created NodePort service
- Connected service to deployment using labels
- Accessed application via browser

### Commands Used
- kubectl apply -f service.yaml
- kubectl get services
- minikube ip
- minikube service

## Kubernetes Day 5 - Deployment + Service

- Combined Deployment and Service in single YAML file
- Deployed multi-pod application
- Exposed app using NodePort service
- Tested scaling and auto-healing

### Architecture
User → Service → Deployment → Pods

### Commands Used
- kubectl apply -f app.yaml
- kubectl get all
- kubectl scale deployment
- kubectl delete pod
- minikube service
