# Define how Tilt should build your Docker image
docker_build('my-service', './')

# Ensure the image is built before running the container
local_resource(
    'run-my-service', 
    'docker run -d --name my-service -p 8888:80 my-service', 
    deps=['./Dockerfile']
)
