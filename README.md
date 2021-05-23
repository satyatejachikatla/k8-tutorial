# k8-tutorial

## Commands

### Start test node

```
minikube start --vm-driver=docker
```

### Info cmds

```
minikube status
kubectl get all
kubectl get node
kubectl get pod
kubectl get deployment
kubectl version
kubectl get replicaset
kubectl logs <pod name>
kubectl describe pod <pod name>
```

### Create deployment

```
kubectl create deployment nginx-depl --image=nginx
kubectl get deployment
kubectl get replicaset
```

### Edit deployment

```
kubectl edit deployment nginx-depl
```

### Enter pod 

```
kubectl exec -it mongo-depl-5fd6b7d4b4-drjjn /bin/bash
```

### Delete

```
kubectl delete deployment mongo-depl
kubectl get deployment
kubectl get pods
```

### Depolyment/Service from config

```
kubectl apply -f <config.file>
kubectl delete -f <config.file>
```

### Service

```
kubectl get service
kubectl describe service <service>
```

### Generated yamls

```
kubectl get deployment -o yaml
kubectl get service -o yaml
```

### Secret/ConfigMap

```
kubectl get secret
kubectl get configmap
```

### Open Service to outside in minicube cluseter
```
minikube service mongo-express-service
```

## Reference

* Tutorial : https://www.youtube.com/watch?v=X48VuDVv0do