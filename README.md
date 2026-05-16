# **\[CS 2600\] Final - Docker**
## Reference
[welcome-to-docker](https://hub.docker.com/r/docker/welcome-to-docker)

## YouTube Video Links
[Docker on Laptop](https://youtu.be/3SGXdswoV0Q)
[Docker on GCP](https://youtu.be/VV4fudXTHmI)

## Commands ran in terminals (local and GCP)
### 1: Pulling the docker image
```docker pull docker/welcome-to-docker:latest```
### 2 + 3: Running and setting up the GCP instance and laptop environment using docker
```sudo apt-get install docker.io```
- I ran this command on the GCP to download it. I already had docker downloaded on my regular laptop environment from class.
### 4: Running the application to get the response
```docker run -d -p 8088:80 --name welcome-to-docker docker/welcome-to-docker```
- This ran the application. On my laptop, I was able to see the application on `http://localhost:8088`.
```docker ps```
- On the GCP instance, I was able to see that the container was running.
```docker stop <Container_ID>```
- On the GCP instance, this command stopped the container.
```docker rm <Container_ID>```
- I used this command to remove the container. This also allowed me to create a new container with the same name if needed.
