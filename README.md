# kentldolarMyWebsite
Bootcamp Training 2020

# Create docker for servers local
create docker file successfully
use nginx virtual for macos

create image
cd docker
docker build -t some-content-nginx .

Exposing external port
docker run --name some-nginx -d -p 8080:80 some-content-nginx
  # Then you can hit http://localhost:8080 or http://host-ip:8080 in your browser.

  # if error occurs
remove all images
docker rmi -f $(docker images -a -q)

remove all containers
docker rm -vf $(docker ps -a -q)


# for windows need vagrant
virtual box ubuntu
use nginx

# Sources:
  # docker
https://stackoverflow.com/questions/44785585/how-to-delete-all-local-docker-images
  # nginx docker
https://hub.docker.com/_/nginx
