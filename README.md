# Baqend Community Edition
Run the Baqend Community Edition and start developing awesome applications in minutes using Docker with Docker Compose. It's free for personal and commercial projects. If you do not want to host and install anything, try the free [Baqend cloud service](https://www.baqend.com/platform.html).

## Quickstart
```bash
$ docker-compose up -d
```

## What is Docker Compose ?
Docker Compose is a tool for defining and running multi-container Docker applications. With Compose, you can define a multi-container application in a single file, which spins up your application in a single command that does everything that needs to be done to get it running.

For more information visit the official Docker documentation : https://docs.docker.com/compose/

## Usage
1. Make sure you have [Docker](https://docs.docker.com/get-started/) and [Docker-Compose](https://docs.docker.com/compose/install/) installed and running on your machine.
2. Copy or checkout the docker-compose.yml from this repository to the directory from which you want to spin up your Baqend server.
3. Run `docker-compose up -d` to spin up your Baqend Server
4. Open [http://localhost:8080/dashboard](http://localhost:8080/dashboard) in your browser
5. Start developing awesome applications

The docker-compose.yml will spin up 3 different containers, that are needed to run your server.
1. `mongo` as a database for persisting your data
2. `orestes` runs the baqend server including the dashboard
3. `node` which runs your custom backend code in addition to orestes
