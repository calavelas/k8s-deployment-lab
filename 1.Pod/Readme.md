# Let's play Pod

Apply Pod
```
kubectl apply -f Pod.yaml
```

Display all pods information
```
kubectl get pods -o wide
```

Test access
```
kubectl port-forward pod/my-pod 8080:80
```

Delete Pod resource
```
kubectl delete -f Pod.yaml
```