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
# Clear Read-Only status and add all permissions for all users
- sudo chmod -R a+rwx dockerSymfony

# Open php bash
- docker exec -it php74-container bash
# Install symfony 
- composer create-project symfony/skeleton .
# Add package.json, webpack and other
composer require encore

# Create DB
- docker-compose run --rm php74-service php bin/console doctrine:database:create
# Open MySQl bash
- docker exec -it mysql8-container bash
# Command in mySQL bash
- mysql -uroot -psecret
- show databases;

# Install npm
- docker-compose run --rm node-service npm install
# Start npm dev
- docker-compose run --rm node-service npm run dev

# For start new project
- symfony composer require http-client doctrine maker phpunit
# For phpunit, reset DB after testing
- composer require --dev dama/doctrine-test-bundle
# For run phpunit test
- symfony php bin/phpunit tests/StockTest.php
