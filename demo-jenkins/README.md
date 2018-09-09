www.play-with-docker.com<br>
<h1>docker run</h1>docker run -it -p 8080:8080 jenkins<br>
<h1>docker-compose with bash</h1>
cd;git clone https://github.com/yoyoware/docker;cd ./docker/demo-jenkins;sudo docker-compose up -d<br>
docker exec -it demo bash
<h1>configure</h1>
the boot page of jenkins will ask you for the default admin password<br>
you can locate the default admin password here:<br>
- shell connect to URL: ssh -l ubuntu -i mykey ec2-34-241-171-75.eu-west-1.compute.amazonaws.com<br>
- locate the jenkins container: sudo docker container ls<br>
- open the jenkins container log: sudo docker logs container_id<br>
- open URL:8080 enter jenkins default admin password
