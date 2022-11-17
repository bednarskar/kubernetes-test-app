# build docker
cd hello-kube
docker build -f docker/Dockerfile -t bednarskar/hello-kube .
docker run -p 8080:8081 -t bednarskar/hello-kube
kubectl apply -f deployment.yml
