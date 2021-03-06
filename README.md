# DOCKER CRASH COURSE

Docker is a software framework for building, running, and managing containers on servers and the cloud.

## 🤔 Why Docker?

- Virtual machines virtualize hardware which seems to be slow and bulky
- Docker is faster since it only virtualizes operating system
- By using isolated containers, if it works here it will work anywhere

<img src="./images/docker-vs-vm.png" alt="Docker vs virtual machines">

## 🛠 Installation

https://docs.docker.com/get-docker/

Simple and easy for Mac and Linux. For Windows, a subsystem for linux called WSL is required.

## 📝 Workflow

<img src="./images/workflow.jpg" alt="Docker workflow">

## 🐳 Docker Hub

<img src="./images/docker-hub.png" alt="Docker hub">

## 🤖 Basic Commands

```sh
docker images
```

```sh
docker ps -a
```

```sh
docker build -t myapp:v1 .
```

```sh
docker run --name myapp_c1 -p 4000:4000 -d --rm myapp:v1
```

```sh
docker run --name myapp_c1 -p 4000:4000 --rm -v /local/path:/app -v /app/node_modules myapp:v1
```

```sh
docker start myapp_c1
```

```sh
docker stop myapp_c1
```

```sh
docker image rm -f myapp
```

```sh
docker container rm myapp_c1 myapp_c2
```

```sh
docker system prune -a
```

```sh
docker-compose up
```

```sh
docker-compose down
```

```sh
docker --rmi all -v
```

## 🏗️ Image to build

https://hub.docker.com/r/honmetha/myapi

```sh
docker pull honmetha/myapi
```

## 📖 Chapters

1. What is Docker?
1. Installing Docker
1. Images & Containers
1. Parent Images & Docker Hub
1. The Dockerfile
1. dockerignore
1. Starting & Stopping Containers
1. Layer Caching
1. Managing Images & Containers
1. Volumes
1. Docker Compose
1. Dockerizing a React App
1. Sharing Images on Docker Hub
