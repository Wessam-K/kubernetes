PODS 

kubectl create deployment --image=nginx nginx-app

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



-------------------------------------------
DEPLOYMENT: 


kubectl create deployment nginx-dep --image=nginx


kubectl describe pod nginx-dep-7ccf5fddd7-jwsk8


Kubectl describe deployment nginx-dep 


#scale 
kubectl scale deployment nginx-dep --replicas=7

kubectl get pods -o wide 

minikube ssh
	
curl 10.244.0.27 >> IP 