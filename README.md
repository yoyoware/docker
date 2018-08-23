below are some quick (one command line) docker demos<br>
<br>
if you don't have an OS running docker, this site provides FREE docker nodes: www.play-with-docker.com<br>
<br>
<h1>nginx</h1>cd;git clone https://github.com/yoyoware/docker;cd docker/demo-nginx;sudo docker-compose up<br>
<br>
<h1>drupal</h1>cd;git clone https://github.com/yoyoware/docker;cd docker/demo-drupal;sudo docker-compose up<br>
URL:8080<br>
configuration: language = english, profile = standard, database = postgres, database name = postgres, database username = postgres, password = mypassword, advanced options host = postgres, site configure page: enter all required fields to your choice<br>
<br>
<h1>jenkins</h1>cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-jenkins;mkdir my-jenkins-data;chmod 777 my-jenkins-data;sudo docker-compose up<br>
URL:8080<br>
configuration: copy/page password from docker install completion page
<br>
<h1>ubuntu ls</h1>cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-ubuntu;sudo docker-compose up<br>
<h1>ubuntu ls</h1>cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-ubuntu;sudo docker-compose up<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<h1>stop & remove all containers, remove dangling volumes</h1>
docker stop $(docker ps -a -q);docker rm $(docker ps -a -q);docker volume prune -f
<br>
<h1>list all containers, images, volumes</h1>
docker container ls;docker images;docker volume ls
<br>
<h1>remove docker tree</h1>
rm -rf docker
<br>
<br>
<h1>git commit</h1>
cd; rm -rf ./docker/demo-jenkins-with-volume/my-jenkins-data;cd ./docker;git config --global user.email "michaelemens@gmail.com";git pull;git add -A; git commit -m "comment"; git push origin master</b>




