# Deploying Kubernetes pods

Kubernetes pods deployed using three ways:
1. **Creating application**: Flask application is created that encompasses itself the communication between the pods: 'Hello World' and 'I got it, roger’
2. **Generating the image using Dockerfile**: Using the Dockerfile, image is generated utilizing the command:
`````
docker build -t [image name] .
``````
3. **Deploying the app**: Deployment.yaml is created which includes both the service and deployment creating 5 number of instances. The service and deployment is created using the following command:
``````
kubectl apply -f deployment.yaml 
