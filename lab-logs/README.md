```
kubectl run nginx --image nginx
```

```
kubectl run nginx --image nginx --dry-run=client -oyaml
```

```
kubectl run nginx --image nginx --dry-run=client -oyaml > test-pod.yaml
```
(optional)
```
kubectl run nginx --image busybox --dry-run=client -oyaml -- sleep infinity > test-pod.yaml
```

```
vim test-pod.yaml
```

```
kubectl create deployment nginx --image nginx
```
```
kubectl get po
```
```
kubectl get deploy
```
**Delete pod and explain replicas. How pod is schduled**
```
kubectl create deployment nginx --image nginx --dry-run=client -oyaml > test-deployment.yaml
```

```
vim test-deployment.yaml
```

to check what can be created
```
kubectl create
```
to check what can be shorten
```
kubectl api-resources
```

explain what is on yaml
what logs it writes
```
kubectl apply -f pod-for-logs.yaml
```

```
kubectl logs <pod name> -n <namespace>
```
