www.play-with-docker.com<br>

# git clone
`cd;rm -rf hack2019;git clone https://github.com/yoyoware/hack2019`

# stop & remove all containers, remove dangling volumes
`docker ps -aq;docker stop $(docker ps -a -q);docker rm $(docker ps -a -q);docker rmi -f $(docker images -q);docker volume prune -f;docker ps -aq`

# list all containers, images, volumes
`docker container ls;docker images;docker volume ls`

# remove docker tree
`rm -rf docker`

# docker build
`cd ~/hack2019;docker build --tag apollo .`<br>
`docker run -it -p 4000:4000 apollo bash`<br>
`node index.js`<br>
paste this into the left side of console: <br>
`{ books { title author } }`<br>

# git commit
`cd;cd ./hack2019;git config --global user.email "michaelemens@gmail.com";git pull;git add -A; git commit -m "comment"; git push origin master`





