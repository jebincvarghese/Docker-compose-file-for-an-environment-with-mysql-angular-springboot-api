# MySQL + Spring Boot + Angular 7 Deployment using Docker Compose

Creating Docker files for Spring boot and Angular. Constructing Docker Compose file to deploy all of them


### Prerequisites

Make sure you have already installed Docker Engine.
You don’t need to install Nginx or NPM, as both are provided by Docker images.

```
$ docker -v
Docker version 18.03.1-ce, build 9ee9f40
```


### Run the Docker-Compose File

So once we have all the components in place, the last thing left to do is just running a simple command.


```
git clone https://github.com/jebincvarghese/Docker-compose-file-for-an-environment-with-mysql-angular-springboot-api.git angular

cd angular

sudo docker-compose up --build -d
```

Make sure you run this command where ever you have created the docker-compose.yml file. The --build is to build the Dockerfile to create fresh images instead of using the existing ones and the -d is to make it run on daemon.

To view the list of services running by this docker-compose we can use this command
```
sudo docker-compose ps
```
Go to [http://localhost](http://localhost)
