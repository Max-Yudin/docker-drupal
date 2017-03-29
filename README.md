# Docker for drupal

## Commands
docker-compose --file ./docker-compose.yml up -d

docker-compose --file ./docker-compose.yml up --build --force-recreate

docker stop $(docker ps -a -q)

docker stop $(docker ps -a -q) && docker rm $(docker ps -a -q)
