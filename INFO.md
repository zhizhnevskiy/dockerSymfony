# Build and run container
- docker-compose up -d --build
# Run container
- docker-compose up
# Server will be start on
- http://localhost:8080/

# Show all started containers 
- docker ps
# Show all containers
- docker ps -a
# Stop all started containers
- docker kill $(docker ps -q)
# Delete all containers
- docker rm $(docker ps -a -q)

# Open php bash
- docker exec -it php74-container bash
# Install symfony 
- composer create-project symfony/skeleton .
