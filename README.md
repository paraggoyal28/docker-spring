# Docker
Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications.

# Container
Simply put, a container is a sandboxed process on your machine that is isolated from all other processes on the host machine.
* Is a runnable instance of an image. You can create, start, stop, move, or delete a container using the DockerAPI or CLI.
* Can be run on local machines, virtual machines or deployed to the cloud.
* Is portable (can be run on any OS).
* Is isolated from other containers and runs its own software, binaries, and configurations.

# Container Image
When running a container, it uses an isolated filesystem. This custom filesystem is provided by a container image. Since the image contains the container’s filesystem, it must contain everything needed to run an application - all dependencies, configurations, scripts, binaries, etc. The image also contains other configuration for the container, such as environment variables, a default command to run, and other metadata.

# Useful commands in docker

1. **docker build -t getting-started .**

The docker build command uses the Dockerfile to build a new container image

2. **docker run -dp 3000:3000 getting-started**

Starting a container 

3. **docker ps**

List all containers

4. **docker stop $container-id$**

Stops the container with given container id. To find the container id use **docker ps**

5. **docker rm $container-id$** 

Removes the container with given container id.

6. **docker tag getting-started YOUR-USER-NAME/getting-started**

Give the container image a new name

7. **docker push YOUR-USER-NAME/getting-started**

Pushing an docker image to dockerhub

