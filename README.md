# Deployment For Deals Application

## Tech

Deals application is developed upon the following projects:
- [Spring Boot] - To develop and deploy rest endpoints
- [MySql] - To persist user and deals information
- [docker-hub] - The built images are deployed to docker hub

## Deployment Procedure

This repository contains the installation scripts to install the web app, messaging server and MySql (master and slave)

MySql is the dependent module for both web application and the messaging server hence you have to start the MySql before starting the web application or messaging server.

Make sure the port 8180, 8181, 5506, 5506

For Starting MySql
```sh
cd mysql
docker-compose up
```


For Starting Messaging Server
```sh
cd messaging-server
docker-compose up
```

For Starting Deals application
```sh
cd web-app
docker-compose up
```