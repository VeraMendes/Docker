# Docker
## Using my package from test pypi in Docker

#### create a new empty directory in Docker called containers: 
mkdir containers

#### enter new directory using: 
cd containers

#### inside this directory, create a new directory for my project called lambdata: 
mkdir lambdata

#### enter new project directory:
cd lambdata

#### create a Dockerfile inside this directory:
touch Dockerfile

#### enter file with nano to introduce the content on **Dockerfile** file in this repo:
nano Dockerfile

#### build the Dockerfile image:
docker build . -t lambdata_veramendes

#### run the docker image:
docker run -it lambdata_veramendes /bin/bash

#### check the folder on your containers:
docker container ls -a

#### open python3 to test my module:
python3

### example of testing:



