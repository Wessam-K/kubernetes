kubectl create deplyment --image=nginx nginx-app

kubectl apply -f helloworld-pod.yml

kubectl get pods

kubectl get all

kubectl get pods -o json

kubectl describe nginx

kubectl exec -it nginx -- /bin/bash

minikube dashboard

kubectl exec -it webserver /bin/bash

kubectl logs nginx


kubectl delete deployment all





apiVersion: v1
kind: Pod
metadata:
  name: webserver
spec:
  containers:
  - name: webserver
    image: nginx:latest
    ports:
    - containerPort: 80