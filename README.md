www.play-with-docker.com<br>
<h1>hello-world</h1>cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-hello-world;sudo docker build -t hello-world:latest .;sudo docker run hello-world<br><br>

<h1>stop & remove all containers, remove dangling volumes</h1>
docker ps -aq;docker stop $(docker ps -a -q);docker rm $(docker ps -a -q);docker rmi $(docker images -q);docker volume prune -f;docker ps -aq
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




