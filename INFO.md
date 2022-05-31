# Show all started containers 
- docker ps
# Show all containers
- docker ps -a
# Stop all started containers
- docker kill $(docker ps -q)
# Delete all containers
- docker rm $(docker ps -a -q)

# Build and run container
- docker-compose up -d --build
# Run container
- docker-compose up