# configmap
```
vim pod-with-configmap.yaml
vim configmap.yaml
```
can change configmap
```
kubectl apply -f pod-with-configmap.yaml
```
errorconfig
```
kubectl apply -f configmap.yaml
```
pod completed
```
kubectl logs dapi-test-pod
```

can change configmap

# empty dir
explain
```
vim pod-with-emptyDir.yaml
```
```
kubectl apply -f pod-with-emptyDir.yaml
```
```
kubectl logs 
```
```
kubectl logs counter
kubectl logs counter count
kubectl logs counter count-log-1
kubectl logs counter count-log-2
```
# pv/pvc

maybe change file name
```
vim pod-with-pvc.yaml
vim pvc.yaml
vim pv.yaml


```
```
kubectl apply -f pod-with-pvc.yaml -f pvc.yaml -f pv.yaml
```
