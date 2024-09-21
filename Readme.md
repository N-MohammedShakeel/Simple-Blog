# Docker Setup

```bash
# Build the Docker image from the Dockerfile
docker build -t blogv .

# Run the container using volumes
docker run --name blog_cv -p 4000:4000 -v d:/udemy/web_development/others/blog:/app -v /app/node_modules blogv:latest

# General format for running Docker containers with volumes
docker run --name <container-name> -p <host-port>:<container-port> -v <sourcecode-folder-path>:<container-folder-path> -v <dependencies-folder-path>:<container-folder-path> <image-name>:<tag>

# Docker Compose: Build the images
docker compose build

# Docker Compose: Start the containers
docker compose up

# Docker Compose: Stop and remove the containers
docker compose down
