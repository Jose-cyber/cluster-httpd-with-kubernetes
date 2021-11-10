# Deploying a cluster with Kubernetes using kind

this code use kubernetes to provide a cluster with 10 replicas of httpd container running.

### require comands:

* $ kind create cluster --name=httpd-cluster
* $ kubectl apply -f k8s/deployment.yml
* $ kubectl apply -f k8s/service.yml
* $ kubectl port-forward service/webserver-service 80:80



after running the requirements commands, you can open this application in your browser and access using:<br>
**http://localhost:80/**
<br>
if you run command: <br>
**kubectl get pods**<br>
you will can see the all pods running
<br>
<img src="https://i.ibb.co/TRHc7pz/Captura-de-tela-de-2021-11-01-02-50-57.png">