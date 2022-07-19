```
kubectl run nginx --image nginx
```

try curl from pod clusterIP
if pod is deleted 
cannot curl the same IP

```
kubectl create deploy nginx --image nginx
```
delete po ip is changed

that's why we have to use svc
```
kubectl expose deploy nginx --port 80
```
maybe draws
how deploy/pod collabs with svc


```
vim ingress.yaml
kubectl apply -f ingress.yaml
kubectl get ingress
```
```
kubectl get svc -n ingress-nginx
```
```
curl -v http://training-worker1/ -H 'Host: foo.bar.com'
curl -v http://training-master/ -H 'Host: foo.bar.com'
```
draws clients > ingress-controller > svc > pod
