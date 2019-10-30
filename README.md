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

```>>> from lambdata_veramendes import RANDINT
>>> RANDINT
    0
0  33
1  31
2  58
3  50
4  41
5   9
6  82
7  28
8  26
9  53
>>> from lambdata_veramendes import Date
>>> Date
<class 'lambdata_veramendes.Date'>
>>> date = Date()
>>> date()
>>> date.get_year()
1900
>>> date.get_month()
1
>>> date.get_day()
1
>>> from lambdata_veramendes import increment
>>> increment(3)
4
