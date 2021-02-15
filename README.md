# Udagram Microservices
## Udacity Cloud Developer Nanodegree

### Getting Started
Udagram is a simple cloud application with 4 Docker Containers
* Feed Service API
* User Service API 
* Front APP
* API Gateway

### Prerequisites
You need to install:
Docker
AWS CLI
Eksctl
AWS-iam-authenticator
Kubectl

 ### Local Instalation
 Run the following docker commands 
```
docker pull nowindi/udagram-user-service-container
docker pull nowindi/udagram-feed-service-container
docker pull nowindi/udagram-api-gateway

docker images //get the new images

dc run --rm -it --name udagram-user-service  -p 8082:8080 <image id>
dc run --rm -it --name udagram-feed-service  -p 8081:8080 <image id>
dc run --rm -it --name udagram-api-gateway  -p 8080:8080 <image id>

git clone https://github.com/nowindi/udagram-ionic-app.git

ionic serve
```