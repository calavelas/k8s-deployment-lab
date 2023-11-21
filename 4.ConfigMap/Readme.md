# Let's play ConfigMap

Apply ConfigMap
```
kubectl apply -f ConfigMap.yaml
```

Display ConfigMap information
```
kubectl describe configmaps my-configmap
```

Apply Pod with environment variable reference ConfigMap
```
kubectl apply -f Pod.yaml
```

Check environment variable in Pod
```
kubectl port-forward pod/my-pod 8080:80
```

Delete Pod
```
kubectl delete -f Pod.yaml
```

Delete ConfigMap
```
kubectl delete -f ConfigMap.yaml
```