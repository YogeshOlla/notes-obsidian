## Dockerfile: 
Text file that serves as an instruction manual for a blueprint

## Docker Image: 
The blueprint for a Docker container. It's immutable, and to make changes, you need to edit the Dockerfile.

## Docker Container: 
A runtime instance of a Docker image. It's isolated, can be replicated, and each replication can be managed independently.

## How to work with Docker:

### 1. Create a Dockerfile:
   - FROM
   - WORKDIR
   - COPY
   - RUN
   - CMD
   - EXPOSE

### 2. Build Docker image:
   `docker build -t <give image a name> .`
   Needs to be run when building the image for the first time or whenever the application file has been edited, so it can be rebuilt.

### 3. Run Docker container:
   `docker run -dp <host>:LocalPort:ContainerPort <image-name>`
   - d: Detached (runs the container in the background)
   - p: Publish (creates port mapping between host and container)
   - host: Address of the host
   E.g., `docker run -dp 127.0.0.1:3000:3000 getting-started`

### 4. Container management:
   - Check running Docker containers: `docker ps`
   - Stop a container: `docker stop <container-id>`
   - Remove a container: `docker rm <container-id>`

### 5. Data Persistence:
   When running a container, if we need to save the data, follow these steps:
   - Create a volume: `docker volume create <name>`
     This volume will run as a separate container and can be deleted similarly using `docker rm -f <container-id>`
   - Mount in the main container: If we want the data to be stored in the volume, we need to mount it.
     `docker run <docker regular command for running> --mount type=volume,src=<name>-db,target=<volume location> <image-name>`
### 6. Network Creation:

To create a network for Docker containers to communicate with each other:

`docker run -d \
`--network my-network \
`-v /path/to/volume:/container/mount \ 
`-e ENV_VARIABLE=value \inside the container \
`-e ANOTHER_ENV_VARIABLE=value \
`sql:latest `

- `docker run -d`: Starts a container in detached mode, meaning it runs in the background.
- `--network my-network`: Attaches the container to the "my-network" network, allowing it to communicate with other containers on that network.
- `-v /path/to/volume:/container/mount`: Mounts a volume from the host machine (`/path/to/volume`) to a directory inside the container (`/container/mount`), allowing for persistent data storage.
- `-e ENV_VARIABLE=value`: Sets an environment variable (`ENV_VARIABLE`) with a specific value (`value`) inside the container.
- `-e ANOTHER_ENV_VARIABLE=value`: Sets another environment variable (`ANOTHER_ENV_VARIABLE`) with a specific value (`value`) inside the container.
- `sql:latest`: Specifies the image to use for creating the container (`sql`) and its tag (`latest`). Adjust this according to your specific image name and tag.


Checked if the container is connected: `docker exec -it <sql container id> <sql name> -u root -p`

### 7.Docker Compose

All the above process can be make shorter using a compose file, it helps in defining and sharing multi container applications using a single YAML file

services:
	image1
	image2
	
volumes:
	volumne_name

start the compose the container: `docker compose up -d`
stop the compose container: `docker compose down`