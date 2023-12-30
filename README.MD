### Apply Configurations one by one 
```
kubectl apply -f mysql-secret.yaml
kubectl apply -f mysql-pv-pvc.yaml
kubectl apply -f mysql-statefulset.yaml
kubectl apply -f mysql-service.yaml
kubectl apply -f wordpress-pv-pvc.yaml
kubectl apply -f wordpress-deployment.yaml
```
### Apply all configurations
`kubectl apply -f directory_name`
### Access website
Get extgernal IP: `kubectl get svc wordpress-service`, and then go to the IP shown in the output to start installing wordpress.