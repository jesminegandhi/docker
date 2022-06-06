DOCKER PROJECT 

To run the docker container :
docker run -d -p 8080:80 -v "$(pwd):/usr/share/nginx/html:ro" --name web01 nginx

Clean-up:
docker rm -f $(docker ps -a -q)
docker rmi -f $(docker images -q)
