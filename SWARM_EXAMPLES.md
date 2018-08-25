#initialize this node as swarm MASTER<br>
docker swarm init --advertise-addr 192.168.0.46

#start other nodes as WORKER<br>
copy/paste swarm token command line to each worker node in swarm

#list all nodes is swarm<br>
docker node ls

#start nginx in the swarm<br>
docker service create --name "rule-the-world" -p 80:80 nginx

#list the services running in the swarm along with replicas<br>
docker service ls

#list the containers running<br>
docker ps

#list the saervices running along with the nodes they are running on<br>
docker service ps rule-the-world

#this line will deploy the image to all available nodes in swarm<br>
docker service create --name "rule-the-world" -p 80:80 --mode global nginx


