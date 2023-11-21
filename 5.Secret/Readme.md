# Let's play Secret

Apply Secret
```
kubectl apply -f Secret.yaml
```

Display Secret information
```
kubectl describe secrets my-secret
```

Get Secret key value
```
kubectl get secret my-secret -o jsonpath='{.data.SECRET_KEY}' | base64 --decode
```

Apply Pod with environment variable reference Secret
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

Delete Secret
```
kubectl delete -f Secret.yaml
```