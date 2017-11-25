# DOCKER ECOSYSTEM

## Imagen and container
### Pull an nginx imagen 
```
docker pull nginx
```
### Create a container 
```
docker run --name mynginx -d -p 8080:80 nginx
```
## Docker hub
### tag the imagen 
```
 docker tag nginx editaxz/mynginx
```
### Login dockehub 
```
docker login
Username:editaxz
Password:*******
```
### Push imagen docker hub
```
docker push editaxz/mynginx
```
### Verify docker hub
```
https://hub.docker.com/
```

## DockerFile
### Edit dockerfile 
```
sudo nano dockerfile
```
### Build dockerfile 
```
docker build -t editaxz/apache .
```
### Create the container
```
docker run --name apache -d -p 90:80 editaxz/apache
```
### Verify apache
```
verify:  localhost:90
```

## Docker Compose
### Edit docker-compose.yml 
```
sudo nano docker-compose.yml
```
### Up docker-compose.yml 
```
docker-compose up
```
### Verify apache
```
verify:  localhost:90
```

## Docker Machine
### Edit docker-compose.yml 
```
docker-machine --version
docker-machine create --driver virtualbox dev
docker-machine ls
docker-machine stop dev
docker-machine start dev
docker-machine ssh dev
docker-machine rm dev
```


