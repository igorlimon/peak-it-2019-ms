# Remove all docker images and containers
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)

# Display containers
 docker ps --format "{{.ID}} | {{.Image}} | {{.Status}} | {{.Ports}}"
 
 # Display images
 docker images --format "{{.ID}} | {{.Repository}}"
