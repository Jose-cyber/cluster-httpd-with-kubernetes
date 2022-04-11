# Deploying a cluster with Kubernetes using kind
This Kubernetes project provides a local cluster with 10 replicas of docker containers running a custom image, that i pushed to my [docker registry](https://hub.docker.com/repository/docker/josecyber/webserver_httpd).

### Required commands:

* $ kind create cluster --name=httpd-cluster
* $ kubectl apply -f k8s/deployment.yml
* $ kubectl apply -f k8s/service.yml
* $ kubectl port-forward service/webserver-service 80:80

After running the requirements commands, you can open this application in your browser and access using:<br>

**http://localhost:80/**

## PROJECT

This project was created based on youtube video class of [full cycle](https://www.youtube.com/c/FullCycle).
