# Docker_test1

*You can test BrainIAK without installing it using Docker:

docker pull brainiak/brainiak
docker run -it -p 8888:8888 -v brainiak:/mnt --name demo brainiak/brainiak

*To run Jupyter notebooks in the running container, try:

python3 -m notebook --allow-root --no-browser --ip=0.0.0.0

*Then visit http://localhost:8888 in your browser and enter the token. Protip: run screen before running the notebook command.

-----------------------------------------------------------------------------

*docker commands 

docker container ls

docker image ls

-----------------------------------------------------------------------------

*go to an image command line 

docker run -d -it (IMAGE) /bin/bash

docker ps -a

docker exec -it (CONTAINER ID) /bin/bash

-----------------------------------------------------------------------------

*Use [docker images] to see the installed images and [docker ps] to see the running images. 

*When you type [docker run] it takes the image, and makes it a living container with a running process. use [docker run -ti <image>:<tag> bash]
  
* Lastly, images have their own set of ids and containers have their own set of ids - they don't overlap. 

----------------------------------------------------------------------------------------------------------

docker pull [sth]

docker images

docker run -d -it [image name] /bin/bash

docker ps -a

docker exec -it [d3b7...] /bin/bash

apt-get update

apt-get-upgrade

install anything....

exit

docker export -o [address/myfile.tar] [d3b7...]

** RUN THE sOFTWARE IN DOCKER

docker import [OPTIONS] [address] [REPOSITORY[:TAG]]

docker run -d -it [image name] /bin/bash

docker ps -a

**** you just need to do this for a running container:

docker exec -it bb0520621b80 /bin/bash

python3 -m notebook --allow-root --no-browser --ip=0.0.0.0
