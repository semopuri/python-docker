# python-docker

Build docker image 

cd python-docker

docker build -t <app-name>:<tag> .

run docker container

docker run test-docker
Hello World


you need use -v option to mount the host volume on the docker container dir 

Below you can see the current working-directory(pwd)/docker-data-dir is mounted on /data dir of docker container

docker run -it -v $PWD/dokcer-data-dir:/data test-docker '/bin/sh'
