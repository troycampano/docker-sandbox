# Build the container
docker build . -t echo/devbox

# View the existing images
docker images

# Run the container
docker run -dit --name devbox01 echo/devbox

# Connect to container
docker exec -it <container id> /bin/bash