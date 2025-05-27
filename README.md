# DevOps-project
Rani Saed
 

minikube stop
minikube start


kubectl port-forward service/backend 5000:5000

kubectl port-forward service/frontend 3000:80

kubectl port-forward service/pgadmin 5050:80


access to the volume : 
kubectl exec -it postgres*******-- bash
psql -U postgres -d shop_inventory
SELECT * FROM products;

TO EXIT : \q



kubectl get pods -o=jsonpath="{range .items[*]}{.metadata.name}{':\t'}{.spec.containers[*].image}{'\n'}{end}"

backend-5bbc5d864f-f89gz:	rani19/gogo-main-backend:latest
frontend-78d846fc66-6tgnf:	rani19/gogo-main-frontend:latest
pgadmin-8595b9cbd6-86959:	dpage/pgadmin4:latest
postgres-85cd6b7565-2dq8q:	postgres:15

