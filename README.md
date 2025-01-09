# Kubernetes
## 
## usefull commands
To start the minikube which is used to run kubernetes on local machine
```
minikube start
```

```
# to check the cluster information
kubectl cluster-info

# to see nodes
kubectl get nodes

# to see namescpaces
kubectl get namespaces
```
To see pods
```
# to see pods in default namespace
kubectl get pods

# to see pods of all namespace
kubectl get pods -A

# to see pods of specific namespace
kubectl get pods -n development
```
```

# to see deployments in default namespace
kubectl get deployments

# to see deployments of all namespace
kubectl get deployments -A
```
```
# to see services in default namespace
kubectl get services

# to see services of all namespace
kubectl get services -A
```
```
# create namespaces where yaml file contain information for creating namespaces
kubectl apply -f namespace.yaml

# delete namespaces where yaml file contain information for creating namespaces
kubectl delete -f namespace.yaml 
```
```
# create deployment where yaml file contain information for creating deployments
kubectl apply -f deployment.yaml

# to remove pods
kubectl delete pod pod-info-development-5cdffc94c-dxhfx -n development
```
To see information
```
kubectl describe pod pod-info-development-5cdffc94c-fp5g7 -n development
```