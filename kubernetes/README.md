# Deploying Kubernetes pods

Kubernetes pods deployed using three ways:
1. **Creating application**: Flask application is created that encompasses itself the communication between the pods: 'Hello World' and 'I got it, roger’
2. **Generate the image using Dockerfile**: Using the Dockerfile, image is generated utilizing the command:
`````
docker build -t [image name] .
``````
