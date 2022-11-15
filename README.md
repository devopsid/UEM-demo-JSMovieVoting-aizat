# Movie Voting App (Javascript) test code changes

## Application Introduction

![alt text](images/app.png "Application screenshot")
<p style="text-align: center;">&#8673 Application's screenshot</p>

The movie voting app collects votes from users on the favourite movies. The app is built with **React.js** (frontend), **Node.js** and **Express** (backend), and **PostgreSQL** database. It also includes End-to-end testing written with **Cypress**.

A simple illustration of the application architecture:

<img src="./images/apparch.png" alt="Application architecture" width="75%"/>

## Docker deployment

The application’s [docker-compose.yml](/docker-compose.yml) file is included in the project, use the **_docker-compose up_** command on the **project's root folder** to deploy the application on Docker.
```
$ docker-compose up --build –d
```

## Kubernetes Deployment

Also included in the project are the application’s yaml files for Kubernetes deployment, accessible in the **“k8s”** folder. While the **“logging”** and **“monitoring”** folders inside the **“k8s”** folder contains yaml files for **ELK stack** logging and **Prometheus** monitoring deployment on Kubernetes. The deployment architecture of the application on Kubernetes is illustrated below. 

<p align="center">
  <img src="./images/appdeploy.png" alt="Application deployment architecture on Kubernetes" width="75%"/>
</p>
<p align="center">&#8673 Application deployment architecture on Kubernetes</p>

<p align="center">
  <img src="./images/elkdeploy.png" alt="Basic ELK stack architecture on Kubernetes" width="75%"/>
</p>
<p align="center">&#8673 Basic ELK stack architecture on Kubernetes</p>

<p align="center">
  <img src="./images/promdeploy.png" alt="Basic Prometheus architecture on Kubernetes" width="75%"/>
</p>
<p align="center">&#8673 Basic Prometheus architecture on Kubernetes</p>
