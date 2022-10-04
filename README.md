# Building Node Application Docker Image

To build the docker image:

```
docker build -t your_docker_username/nodejs-image-demo .
```

To push to the docker registry:

```
docker push your_docker_username/nodejs-image-demo
```

To create and run a container from the image built and deployed to deocker registry:

```
docker run --name nodejs-image-demo -p 80:8080 -d your_docker_username/nodejs-image-demo
```

To check the logs of the running container:

```
docker logs CONTAINER_ID
```

Add the flag -f to follow the logs

To access the applications's front-end while the container is running, browse to http://localhost in your browser

To stop the app:

```
docker stop CONTAINER_ID
```