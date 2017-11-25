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


