# Remove all docker images and containers
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
