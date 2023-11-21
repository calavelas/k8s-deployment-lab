# Let's play services

### Deployments

Apply Deployment
```
kubectl apply -f Deployment.yaml
```
---

### ClusterIP Service

Apply ClusterIP service
```
kubectl apply -f ClusterIP-svc.yaml
```

Disply all services information
```
kubectl get svc -o wide
```

Test access ClusterIP service
```
kubectl proxy
```
```
http://localhost:8001/api/v1/namespaces/<namespace_name>/services/<service_name>:<service_port>/proxy/
```

---

### Delete Resources

Delete ClusterIP service
```
kubectl delete -f ClusterIP-svc.yaml
```

Delete deployments
```
kubectl delete -f Deployment.yaml
```