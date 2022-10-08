# Build the container
docker build . -t troy/<imagename>

# View the existing images
docker images

# Run the container
docker run -p 49160:8080 -d troy/node-web-app
docker run -dit troy/node-web-app

# View running containers
docker ps

# View all containers
docker ps -a

# Start existing container
docker start <containerid>

# View the logs of the container
docker logs <container id>

# Enter the container
$ docker exec -it <container id> /bin/bash

# Hit the web service

curl -i localhost:49160

# Stop all running containers
docker stop $(docker ps -aq)

# Remove all containers
docker rm $(docker ps -aq)

# Remove all images
docker rmi $(docker images -q)