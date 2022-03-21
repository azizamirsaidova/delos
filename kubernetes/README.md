# Deploy MongoDB with Kubernetes
Python Flask application that communicates MongoDB, containerizing with Docker and Deploying using the Kubernetes. 

This tasks follows three main steps:

1. **Create the application:** Flask application is run in app.py file.
````````````````
* requirements.txt  - Flask, Flask-PyMongo
* app.py - Flask application is run in this Python file
````````````

2. **Containerize the application:** Docker image of the app is created in this stage where docker image is build using the Dockerfile, and pushed to the DockerHub. My DockerHub login is azizamir.


3. **Deployment the application:** Kubernetes cluster is deployed using the minikube

In order to deploy the application, ```.yaml``` is created. ```Taskapp.yaml``` is created using kubectl create.
Kubetcl pods:
<img width="508" alt="Screen Shot 2022-03-21 at 3 43 23 PM" src="https://user-images.githubusercontent.com/57295556/159351575-419d87eb-02ab-48e9-81ca-ed238e523c0e.png">

Deployment is  scaled using kubectl scale.
Kubectl deployments: 
<img width="495" alt="Screen Shot 2022-03-21 at 3 45 02 PM" src="https://user-images.githubusercontent.com/57295556/159351846-6017fdfb-ac93-45bb-b82d-74b07cfe6723.png">

```taskapp-serv.yaml``` service is defined. 
4. **MongoDB deployment and service is created:** 



