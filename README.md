# Prerequisite

Install Gcloud CLI

```
brew install --cask google-cloud-sdk
```

\
Install kubectl and auth plugin

```
gcloud components install kubectl
```
```
gcloud components install gke-gcloud-auth-plugin
```

\
GKE Cluster Access by gcloud
```
gcloud container clusters get-credentials gke-arise-incubator-lab --region asia-southeast1 --project arise-incubator
```

\
Kube Context
```
kubectl config current-context
```

\
Cluster Info
```
kubectl cluster-info
```
```
kubectl get nodes
```

\
Namespace
```
kubectl get namespace
```
```
kubectl create namespace <namespace_name>
```
```
kubectl config set-context --current --namespace=<namespace_name>
```