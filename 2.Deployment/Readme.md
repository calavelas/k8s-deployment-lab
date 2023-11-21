# Let's play deployment

Apply Deployment
```
kubectl apply -f Deployment.yaml
```

Display all Deployments information
```
kubectl get deployments -o wide
```

Display all Pods information
```
kubectl get pods -o wide
```

Delete Pod for test self healing feature
```
kubectl delete pods <POD_NAME>
```

Scale deployments replicas
```
kubectl scale deployments my-deployment-nginx --replicas=<REPLICAS_COUNT>
```

Delete deployment
```
kubectl delete -f Deployment.yaml
```