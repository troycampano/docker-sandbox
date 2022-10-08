# Build the container

docker build . -t troy/node-web-app

# View the existing images

docker images

# Run the container

docker run -p 49160:8080 -d troy/node-web-app
# docker run -dit troy/node-web-app

# View running containers

docker ps

# View the logs of the container

docker logs <container id>

# Enter the container

$ docker exec -it <container id> /bin/bash

# Hit the web service

curl -i localhost:49160
