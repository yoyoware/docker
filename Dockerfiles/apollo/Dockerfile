#Best practices for writing Dockerfiles
#https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#cmd

#STEPS
#install docker
#pull docker repo
#cd; cd docker/Dockerfiles;cd apollo;docker build --tag apollo .;docker run --rm -it apollo bash

FROM ubuntu:latest

RUN apt-get update && apt-get install -y git && apt-get install -y npm
    
CMD ["git", "--version"]
