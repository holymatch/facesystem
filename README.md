# Face Recognition System

#### Docker status
+ Face Information Server
[![Face Information Server Docker Image](https://dockerbuildbadges.quelltext.eu/status.svg?organization=holymatch&repository=faceweb)](https://hub.docker.com/r/holymatch/faceweb/)
+ Face Engine
[![Face Engine Docker Image](https://dockerbuildbadges.quelltext.eu/status.svg?organization=holymatch&repository=faceengine)](https://hub.docker.com/r/holymatch/faceengine/)


### Introduction
This docker compose file is used for setup Face Information Server as well as Face Engine in same server at same time.
The Face Recognition System request the following component:
+ [Docker](https://docs.docker.com/)
+ [Docker Compose](https://docs.docker.com/compose/)

## Install facesystem

### Install Docker
To install [Docker CE](https://docs.docker.com/install/#releases) please follow the instruction to install the docker.
### Install Docker Compose
To install [Docker Compose](https://docs.docker.com/compose/install/#install-compose) please following the instructions to install the docker compose
### Download facesystem
Download the docker-compose.yml or run the `git clone https://github.com/holymatch/facesystem.git` to download it.




### Run the Server
To run the server run the following command in the root directory of facesystem
```sh
docker-compose up -d
```

To stop the server run the following command in the root directory of facesystem
```sh
docker-compose down
```

### Access the server
The docker will map the port 8080 to the system, use `http://{serverip}:8080/faceweb` to access the server, the Face Information Server also implement Swagger 2, use `http://{serverip}:8080/swagger-ui.html` to access swagger page.
