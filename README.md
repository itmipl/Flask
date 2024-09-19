Build the Docker Image using the Dockerfile
docker build -t hello-world .
Push the Docker Image to Docker Hub
docker tag hello-world <dockerhub-username>/hello-world
docker push <dockerhub-username>/hello-world
Create a Deployment
kubectl apply -f k8s/deployment.yaml
Create service for the Deployment
kubectl apply -f k8s/service.yaml
Create Ingress
kubectl apply -f k8s/ingress.yaml
