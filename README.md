# peak-it-2019-ms
# Remove all docker images and containers
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
