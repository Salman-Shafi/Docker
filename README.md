# Docker Basic Operations

[how-to-remove-docker-images-containers-volumes-and-networks](https://linuxize.com/post/how-to-remove-docker-images-containers-volumes-and-networks/)

### Install Docker Images
cd [your project]
docker run -it --rm --name spfx-helloworld -v %cd%:/usr/app/spfx -p 5432:5432 -p 4321:4321 -p 35729:35729 waldekm/spfx

### Execute container
docker exec -it spfx-helloworld /bin/bash 

### Pull Latest Docker Image of 'waldekm/spfx'
docker pull waldekm/spfx:latest

### List all images
docker image ls

### List all containers
docker container ls

### Stop container by container id
docker container stop <container_id>

### Remove container by container id
docker container rm <container_id>

### If don't want stop and remove, can force remove
docker container rm -f <container_id>

### Remove image
docker image rm <image_id>
