## Minikube
Start Minikube
```
minikube start
```

<br>

Run minikube tunnel to expose an external ip for api-gateway's LoadBalancer service (this process must stay alive in terminal)
```
minikube tunnel
```

<br>

Apply files (images must be exists in the minikube container)
```
kubectl apply -f redis.yaml -f market-service -f crypto-service -f auth-service -f api-gateway
```
