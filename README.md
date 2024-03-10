Task 2
```
kubectl apply -f mysql_pod.yaml -n database
```
```
kubectl describe pod/mysql -n database
```
```
10-244-0-13.database.pod.cluster.local
```

```
kubectl apply -f app_pod.yaml -n webapp
```

```
kubectl get all pods -n webapp
```
```
kubectl port-forward web-app 8080:8080 -n webapp
```
In the new termial
```
curl localhost:8080
```

logs
```
kubectl logs web-app -n webapp
```
```
kubectl logs mysql -n database
```
