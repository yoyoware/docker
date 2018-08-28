#Best practices for writing Dockerfiles
#https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#cmd
#cd /docker/Dockerfiles;docker build --tag sample-1 .;docker run --rm -it sample-1 bash

FROM ubuntu:latest

RUN apt-get update 
#&& apt-get install -y \
#    git
    
CMD ["git", "--version"]
