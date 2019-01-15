www.play-with-docker.com<br>

# git clone
cd; rm -f docker;git clone https://github.com/yoyoware/docker

# stop & remove all containers, remove dangling volumes
docker ps -aq;docker stop $(docker ps -a -q);docker rm $(docker ps -a -q);docker rmi $(docker images -q);docker volume prune -f;docker ps -aq<br>

# list all containers, images, volumes
docker container ls;docker images;docker volume ls<br>

# remove docker tree
rm -rf docker<br>

# git commit
cd;cd ./docker;git config --global user.email "michaelemens@gmail.com";git pull;git add -A; git commit -m "comment"; git push origin master</b>




