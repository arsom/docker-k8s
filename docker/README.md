# Docker 

## https://labs.play-with-docker.com

>docker run -itd -p 80:80 nginx 

>docker ps 

>docker rm -f  [name/container_id]

## fix name 

>docker run --name=test -itd -p 80:80 nginx 

> docker rm -f test

## change port 
> docker run --name=changeport -itd -p 8081:80 nginx 

# docker volumn (mount data from machine to container)
> docker run --name=mount -itd -p 80:80 -v /root/docker-k8s/lab/docker/lab1/:/usr/share/nginx/html nginx 

# build image from docker file 
> docker build -t [name] .
