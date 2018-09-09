www.play-with-docker.com<br>
<h1>docker run</h1>docker run -it -p 80:80 nginx<br>
<h1>docker-compose with bash</h1>
cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-nginx;sudo docker-compose up -d<br>
docker exec -it demo bash


simple dockerfile file that prints hello world when image is run

docker build . -t hello-world:latest
docker run 
