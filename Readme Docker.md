# Create a Dockerfile for Python

`docker init`

`uvicorn 'app.main:app' --bind=0.0.0.0:8000`

# Build an image

`docker build --tag python-docker .`

`docker build --tag python-docker:v1.0.1 .`

## View local images

`docker images`

## Tag images

`docker tag python-docker:latest python-docker:v1.0.0`

## Remove the tag

`docker rmi python-docker:v1.0.0`

# Run your image as a container

`docker run python-docker:v1.0.1`

## To publish a port for your container

`docker run --publish 8000:8000 python-docker`

`docker run -d --name python-docker-container -p 8000:8000 python-docker`
