cd [your project]
docker run -it --rm --name spfx-helloworld -v %cd%:/usr/app/spfx -p 5432:5432 -p 4321:4321 -p 35729:35729 waldekm/spfx
docker exec -it spfx-helloworld /bin/bash 



docker pull waldekm/spfx:latest





<!-- List all containers -->
docker container ls

<!-- List all images -->
docker image ls

<!-- Stop container by container id -->
docker container stop <container_id>

<!-- Remove container by container id -->
docker container rm <container_id>

<!-- If don't want stop and remove, can force remove -->
docker container rm -f <container_id>

<!-- Remove image -->
docker image rm <image_id>
